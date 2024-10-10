# Http - Prompt For OTP
## Configuration
ID:  qdsmqnczwr

Type: CONNECTION 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 


## Custom HTML
```html
<div
    class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">
    <div class="mh-100" style="max-width: 400px; width: 100%;">
        <div class="card shadow mb-5">
            <div class="card-body p-5 d-flex flex-column">
                {{global.parameters.ciam_companyLogo}}
                <h1 class="text-center mb-4">
                    {{#ifEquals type "SMS"}}
                    <i class="mdi mdi-comment-text-outline text-dark fs-1" aria-hidden="true"></i>
                    Text message
                    {{/ifEquals}}
                    {{#ifEquals type "EMAIL"}}
                    <i class="mdi mdi-email-outline text-dark fs-1" aria-hidden="true"></i>
                    Email
                    {{/ifEquals}}
                </h1>
                <p class="text-muted text-center">
                    {{#ifEquals type "SMS"}}
                    Please enter the passcode you received.
                    {{/ifEquals}}
                    {{#ifEquals type "EMAIL"}}
                    Enter the passcode you received to complete email pairing.
                    {{/ifEquals}}
                </p>
                <div id="error-wrap">
                    <p class="text-danger mdi mdi-alert-circle" data-id="feedback" data-skcomponent="skerror"
                        id="error-msg"></p>
                </div>
                <p class="text-danger mdi mdi-alert-circle" data-skerrorid="passcode" data-skcomponent="skerrormessage"></p>
                <form id="otp-form" data-id="otp-form">
                    <div class="mb-4 form-floating">
                        <input class="form-control" id="passcode" type="text" autocomplete="on" maxlength="6" />
                        <label class="form-label" for="passcode">Passcode</label>
                    </div>
                    <p class="text-muted text-center">
                        {{#ifEquals type "SMS"}}
                        Message sent to:
                        {{local.o3p0lu1ww2.payload.output.maskedPhone}}
                        {{/ifEquals}}
                        {{#ifEquals type "EMAIL"}}
                        Email sent to:
                        {{local.o3p0lu1ww2.payload.output.maskedEmail}}
                        {{/ifEquals}}
                    </p>
                    <div class="d-flex flex-column">
                        <button id="resend" type="button" class="btn btn-link mb-3" data-skcomponent="skbutton"
                            data-skbuttontype="next-event" data-skbuttonvalue="resend">
                            Resend passcode
                        </button>
                        <button id="submit" type="submit" class="btn btn-primary mb-3" data-skcomponent="skbutton"
                            data-skbuttontype="form-submit" data-skform="otp-form" data-skbuttonvalue="submit">
                            Finish
                        </button>
                        <button id="cancel" type="button" class="btn btn-link" data-skcomponent="skbutton"
                            data-skbuttontype="next-event" data-skform="otp-form" data-skbuttonvalue="cancel">
                            Cancel
                        </button>
                    </div>
                </form>
                {{#ifEquals type "SMS"}}
                <p class="text-muted text-center mt-3">I agree to receive a one-time passcode. Message and data rates may
                    apply. Reply STOP to unsubscribe.
                </p>
                {{/ifEquals}}
            </div>
        </div>
    </div>
</div>
```

## Custom Script
```js
const passcode = document.getElementById("passcode");

if (window.addEventListener) {
   // Normal browsers
   errorDiv.addEventListener(&#39;DOMSubtreeModified&#39;, contentChanged, false);
} else if (window.attachEvent) {
   // IE
   errorDiv.attachEvent(&#39;DOMSubtreeModified&#39;, contentChanged);
}

function contentChanged() {
   let errorMsg = document.getElementById(&#39;error-msg&#39;);
   if (errorMsg) {
      errorDiv.classList.add("feedback");
      if (errorMsg.innerText === "OTP Resent") {
         errorMsg.classList.add("feedback--alert");
         errorMsg.classList.add("picon-alert");
         errorMsg.classList.remove("feedback--error");
         errorMsg.classList.remove("picon-error");
      } else {
         errorMsg.classList.remove("feedback--alert");
         errorMsg.classList.remove("picon-alert");
         errorMsg.classList.add("feedback--error");
         errorMsg.classList.add("picon-error");
      }
   } else {
      errorDiv.classList.remove("feedback");
   }
}

```

### Additional Properties
formFieldsList
 ```json 

```


inputSchema
 ```json 
{
    "type": "object",
    "properties": {
        "type": {
            "displayName": "type",
            "preferedControlType": "textField",
            "enableParameters": true
        }
    }
}
```


outputSchema
 ```json 

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
        "url": "deviceType",
        "data": "{{local.eh45uuo9ep.payload.output.deviceType}}",
        "tooltip": "{{local.eh45uuo9ep.payload.output.deviceType}}",
        "children": [
          {
            "text": "deviceType"
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
| [xceoebu0xh](./xceoebu0xh.md) | [wtcsrlx6i1](./wtcsrlx6i1.md) |