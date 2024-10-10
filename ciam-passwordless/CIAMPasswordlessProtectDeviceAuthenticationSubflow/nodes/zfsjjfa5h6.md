# Http - Present FIDO2 Form 
## Configuration
ID:  zfsjjfa5h6

Type: CONNECTION 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 

## Custom CSS
```css
.hidden-button{
    display: none;
}
```

## Custom HTML
```html
<div
    class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">
    <div class="mh-100" style="max-width: 400px; width: 100%;">
        <div class="card shadow mb-5">
            <div class="card-body p-5 d-flex flex-column">
               {{global.parameters.ciam_companyLogo}}
                <h1 class="text-center mb-4">
                    {{#ifEquals type "FIDO2"}}
                    <svg viewBox="0 0 27 26" role="presentation" style="width: 20px; height: 20px;">
                        <path
                            d="M10.2632 12.3158C13.6641 12.3158 16.4211 9.55881 16.4211 6.15789C16.4211 2.75698 13.6641 0 10.2632 0C6.86225 0 4.10527 2.75698 4.10527 6.15789C4.10527 9.55881 6.86225 12.3158 10.2632 12.3158Z"
                            fill="#3D454D" />
                        <path
                            d="M26.6842 12.3158C26.6842 9.67474 24.5631 7.51263 21.9084 7.51263C19.2674 7.51263 17.1053 9.63369 17.1053 12.2884C17.1053 14.1495 18.1589 15.8326 19.8421 16.6263V23.9474L21.8947 26L25.3158 22.5789L23.2631 20.5263L25.3158 18.4737L23.6189 16.7768C25.4663 16.0653 26.6842 14.2863 26.6842 12.3158ZM21.8947 12.3158C21.1421 12.3158 20.5263 11.7 20.5263 10.9474C20.5263 10.1947 21.1421 9.57895 21.8947 9.57895C22.6474 9.57895 23.2631 10.1947 23.2631 10.9474C23.2631 11.7 22.6474 12.3158 21.8947 12.3158Z"
                            fill="#3D454D" />
                        <path
                            d="M15.6547 15.08C14.6011 14.6147 13.4653 14.3684 12.3158 14.3684H8.21053C3.68105 14.3684 0 18.0495 0 22.5789V25.3158H17.7895V17.7758C16.8726 17.0642 16.1337 16.1474 15.6547 15.08Z"
                            fill="#3D454D" />
                    </svg>
                    Biometrics/Security Key
                    {{/ifEquals}}
                </h1>
                <p class="text-muted text-center">
                    Follow the directions your browser provides to finish
                    {{#ifEquals type "FIDO2"}} Biometrics/Security Key {{/ifEquals}}
                    authentication.
                </p>
                <p class="text-danger mdi mdi-alert-circle" data-id="feedback" data-skcomponent="skerror"></p>
                <form id="error-form" data-id="error-form">
                    <button class="hidden-button" data-skcomponent="skbutton" data-skbuttontype="form-submit"
                        data-skform="error-form" data-skbuttonvalue="InvalidStateError" id="errorButton">
                        Next
                    </button>
                </form>
                <div class="d-flex flex-column mt-5">
                    <button id="fidoButton" class="btn btn-primary mb-3">
                        Retry
                    </button>
                </div>
                <form id="fido-form" data-id="fido-form" class="d-flex flex-column">
                    <input type="hidden" name="assertionValue" id="assertionValue" />
                    <button class="hidden-button" data-skcomponent="skbutton" data-skbuttontype="form-submit"
                        data-skform="fido-form" data-skbuttonvalue="submit" id="assertionButton">
                        Next
                    </button>
                    {{#if canChangeDevice}}
                    <button id="cancel" class="btn btn-link" data-skcomponent="skbutton" data-skbuttontype="next-event"
                        data-skform="fido-form" data-skbuttonvalue="cancel">
                        Cancel
                    </button>
                    {{/if}}
                </form>
            </div>
        </div>
    </div>
</div>
```

## Custom Script
```js
var authAbortController = window.PublicKeyCredential ? new AbortController() : null;
var authAbortSignal = window.PublicKeyCredential ? authAbortController.signal : null;

window.abortWebAuthnSignal = function abortWebAuthnSignal() {
        authAbortController.abort();
        authAbortController = new AbortController();
        authAbortSignal = authAbortController.signal;
}

window.IsWebAuthnSupported = function IsWebAuthnSupported() {
        if (!window.PublicKeyCredential) {
                console.log("Web Authentication API is not supported on this browser.");
                return false;
        }
        return true;
}

window.isWebAuthnPlatformAuthenticatorAvailable = function isWebAuthnPlatformAuthenticatorAvailable() {
        var timer;
        var p1 = new Promise(function (resolve) {
                timer = setTimeout(function () {
                        resolve(false);
                }, 1000);
        });
        var p2 = new Promise(function (resolve) {
                if (IsWebAuthnSupported() &amp;&amp; window.PublicKeyCredential.isUserVerifyingPlatformAuthenticatorAvailable) {
                        resolve(
                                window.PublicKeyCredential.isUserVerifyingPlatformAuthenticatorAvailable().catch(function (err) {
                                        console.log(err);
                                        return false;
                                }));
                }
                else {
                        resolve(false);
                }
        });
        return Promise.race([p1, p2]).then(function (res) {
                clearTimeout(timer);
                return res;
        });
}
window.WebAuthnPlatformAuthentication = function WebAuthnPlatformAuthentication(publicKeyCredentialRequestOptions) {
        return new Promise(function (resolve, reject) {
                isWebAuthnPlatformAuthenticatorAvailable().then(function (result) {
                        if (result) {
                                resolve(Authenticate(publicKeyCredentialRequestOptions));
                        }
                        reject(Error("UnSupportedBrowserError"));
                });
        });
}
function Authenticate(publicKeyCredentialRequestOptions) {
        return new Promise(function (resolve, reject) {
                var options = JSON.parse(publicKeyCredentialRequestOptions);
                var publicKeyCredential = {};
                publicKeyCredential.challenge = new Uint8Array(options.challenge);
                if (&#39;allowCredentials&#39; in options) {
                        publicKeyCredential.allowCredentials = credentialListConversion(options.allowCredentials);
                }
                if (&#39;rpId&#39; in options) {
                        publicKeyCredential.rpId = options.rpId;
                }
                if (&#39;timeout&#39; in options) {
                        publicKeyCredential.timeout = options.timeout;
                }
                if (&#39;userVerification&#39; in options) {
                        publicKeyCredential.userVerification = options.userVerification;
                }
                navigator.credentials.get({ "publicKey": publicKeyCredential })
                        .then(function (assertion) {
                                // Send new credential info to server for verification and registration.
                                var publicKeyCredential = {};
                                if (&#39;id&#39; in assertion) {
                                        publicKeyCredential.id = assertion.id;
                                }
                                if (&#39;rawId&#39; in assertion) {
                                        publicKeyCredential.rawId = toBase64Str(assertion.rawId);
                                }
                                if (&#39;type&#39; in assertion) {
                                        publicKeyCredential.type = assertion.type;
                                }
                                var response = {};
                                response.clientDataJSON = toBase64Str(assertion.response.clientDataJSON);
                                response.authenticatorData = toBase64Str(assertion.response.authenticatorData);
                                response.signature = toBase64Str(assertion.response.signature);
                                response.userHandle = toBase64Str(assertion.response.userHandle);
                                publicKeyCredential.response = response;
                                resolve(JSON.stringify(publicKeyCredential));
                                document.getElementById("assertionValue").value = JSON.stringify(publicKeyCredential);

                                document.getElementById(&#39;assertionButton&#39;).click();
                        }).catch(function (err) {
                                // No acceptable authenticator or user refused consent. Cancel authentication
                                // if this is the only device so we don&#39;t loop
                                console.log("No acceptable authenticator or user refused consent");

                        });
        });
}
function credentialListConversion(list) {
        var credList = [];
        for (var i = 0; i < list.length; i&#43;&#43;) {
                var cred = {
                        type: list[i].type,
                        id: new Uint8Array(list[i].id)
                };
                if (list[i].transports) {
                        cred.transports = list[i].transports;
                }
                credList.push(cred);
        }
        return credList;
}
function toBase64Str(bin) {
        return btoa(String.fromCharCode.apply(null, new Uint8Array(bin)));
}

const fidoButton = document.getElementById("fidoButton");
fidoButton.addEventListener("click", startFido);
function startFido() {
        Authenticate(&#39;{{{skjson publicKeyCredentialCreationOptions}}}&#39;);
}
fidoButton.click();
```

### Additional Properties
canChangeDevice
 ```json 
[
  {
    "children": [
      {
        "text": ""
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "teleport.svg",
        "url": "canChangeDevice",
        "data": "{{local.7vpjww2ek2.payload.output.canChangeDevice}}",
        "tooltip": "{{local.7vpjww2ek2.payload.output.canChangeDevice}}",
        "children": [
          {
            "text": "canChangeDevice"
          }
        ]
      },
      {
        "text": ""
      }
    ]
  }
]
```


formFieldsList
 ```json 

```


inputSchema
 ```json 
{
    "type": "object",
    "properties": {
        "type": {
            "displayName": "device type",
            "preferedControlType": "textField",
            "enableParameters": true
        },
        "publicKeyCredentialCreationOptions": {
            "displayName": "credentials",
            "preferedControlType": "textField",
            "enableParameters": true
        },
        "canChangeDevice": {
            "displayName": "more then one usable device",
            "preferedControlType": "textField",
            "enableParameters": true
        }
    }
}
```


outputSchema
 ```json 
{
	"type": "object",
	"properties": {
		"buttonValue": {
			"type": "string",
			"propertyName": "buttonValue"
		},
		"assertionValue": {
			"type": "string",
			"propertyName": "assertionValue"
		}
	}
}
```


publicKeyCredentialCreationOptions
 ```json 
[
  {
    "children": [
      {
        "text": ""
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "teleport.svg",
        "url": "publicKeyCredentialCreationOptions",
        "data": "{{local.7vpjww2ek2.payload.output.publicKeyCredentialCreationOptions}}",
        "tooltip": "{{local.7vpjww2ek2.payload.output.publicKeyCredentialCreationOptions}}",
        "children": [
          {
            "text": "publicKeyCredentialCreationOptions"
          }
        ]
      },
      {
        "text": ""
      }
    ]
  }
]
```


type
 ```json 
[
  {
    "children": [
      {
        "text": ""
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "teleport.svg",
        "url": "type",
        "data": "{{local.7vpjww2ek2.payload.output.type}}",
        "tooltip": "{{local.7vpjww2ek2.payload.output.type}}",
        "children": [
          {
            "text": "type"
          }
        ]
      },
      {
        "text": ""
      }
    ]
  }
]
```


undefined
 ```json 

```


validationRules
 ```json 

```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [t04dles3gs](./t04dles3gs.md) | [9pb86bg0qi](./9pb86bg0qi.md) |