# Http - Gather Browser Information
## Configuration
ID:  na4hef71sq

Type: CONNECTION 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 

## Custom CSS
```css
.hidden-button {
  display: none;
}
```

## Custom HTML
```html
<!-- Check whether the end-user browser is supporting WebAuthn to understand if security keys and platform biomentic method are usable -->
<form id="webAuthenSupportForm" method="post">
    <input type="hidden" name="webAuthenSupport" id="webAuthenSupport">
    <button type="hidden" data-skcomponent="skbutton" data-skbuttontype="form-submit" class="hidden-button"  data-skbuttonvalue="submit" data-skform="webAuthenSupportForm" id="autoSubmit">Next</button>
</form>
```

## Custom Script
```js
function isWebAuthnSupported() {
    try {
        if (!window.PublicKeyCredential) {
            console.log("Web Authentication API is not supported on this browser.");
            return false;
        }
        return true;
    } catch (error) {
        console.log(error);
        return false;
    }
}

function isWebAuthnPlatformAuthenticatorAvailableV2() {

    var timer;

    var isTimeout = false;

    var p1 = new Promise(function (resolve) {
        timer = setTimeout(function () {
            console.log("isWebAuthnPlatformAuthenticatorAvailable - Timeout");
            isTimeout = true;
            resolve(false);
        }, 1500);
    });

    var p2 = new Promise(function (resolve) {

        if (isWebAuthnSupported() &amp;&amp; window.PublicKeyCredential.isUserVerifyingPlatformAuthenticatorAvailable) {

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
        console.log("isWebAuthnPlatformAuthenticatorAvailable - " &#43; res);

        return { supported: res, timeout: isTimeout };
    });
}

setTimeout(function () {
    const authSuported = isWebAuthnSupported();
    isWebAuthnPlatformAuthenticatorAvailableV2().then(function (result) {
        document.forms[&#39;webAuthenSupportForm&#39;].elements["webAuthenSupport"].value = result.supported ? "FULL" : (authSuported ? "SECURITY_KEY_ONLY" : "NONE");
        document.getElementById(&#39;autoSubmit&#39;).click();
    }).catch(function (err) {
        document.forms[&#39;webAuthenSupportForm&#39;].elements["webAuthenSupport"].value = authSuported ? "SECURITY_KEY_ONLY" : "NONE";
        document.getElementById(&#39;autoSubmit&#39;).click();
    });
}, 400);
```

### Additional Properties
formFieldsList
 ```json 

```


inputSchema
 ```json 

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
		"webAuthenSupport": {
			"type": "string",
			"propertyName": "webAuthenSupport"
		}
	}
}
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
| [p8n9w6rdgy](./p8n9w6rdgy.md) | [tir7r8fvkp](./tir7r8fvkp.md) |