# Http - string 
Prompt For OTP
## Configuration
ID:  79cmhtu9fy

Type: CONNECTION 

CapabilityName: customHTMLTemplate


## Custom CSS
```css
json 
.form-control {
    padding-top: 0rem !important;
    padding-bottom: 0rem !important;
    font-size: 17px;
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
                    {{#ifEquals type "EMAIL"}}
                    <i class="mdi mdi-email-outline text-dark fs-1" aria-hidden="true"></i>
                    Email
                    {{/ifEquals}}
                </h1>
                <p class="text-muted text-center">
                    {{#ifEquals type "EMAIL"}}
                    Enter the passcode you received.
                    {{/ifEquals}}
                </p>
                <div id="error-wrap">
                    <p class="text-danger mdi mdi-alert-circle text-center" data-id="feedback" data-skcomponent="skerror"
                        id="error-msg"></p>
                </div>
                <p class="text-danger mdi mdi-alert-circle text-center" data-skerrorid="passcode" data-skcomponent="skerrormessage"></p>
                <form id="otp-form" data-id="otp-form">
                    <div class="mb-4 form-floating">
                        <input class="form-control text-center" id="passcode" type="text" autocomplete="on" maxlength="6" />
                    </div>
                    <div class="d-flex flex-column mt-5">
                        <button id="resend" type="button" class="btn btn-link" data-skcomponent="skbutton"
                            data-skbuttontype="next-event" data-skbuttonvalue="resend">
                            {{#ifEquals type "EMAIL"}}
                            Resend Passcode
                            {{/ifEquals}}
                
                        </button>
                        <button id="submit" type="submit" class="btn btn-primary mb-3" data-skcomponent="skbutton"
                            data-skbuttontype="form-submit" data-skform="otp-form" data-skbuttonvalue="submit">
                            Submit OTP
                        </button>
                        {{#unless disableCancel}}
                        <button id="cancel" type="button" class="btn btn-link" data-skcomponent="skbutton"
                            data-skbuttontype="next-event" data-skform="otp-form" data-skbuttonvalue="cancel">
                            Cancel
                        </button>
                        {{/unless}}
                    </div>
                </form>
            </div>
        </div>
    </div>
</div>
```

## Custom Script
```js 
const passcode = document.getElementById("passcode");
const focusOnFirstInputElement = () => {
  document.getElementById("passcode").focus();
};

var errorDiv = document.getElementById(&#39;error-wrap&#39;);
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

if (document.readyState === "loading") {
  // Loading hasn&#39;t finished yet
  document.onreadystatechange = () => {
    if (document.readyState === "complete") {
      focusOnFirstInputElement(); 
    }
  };
} else {
  // `DOMContentLoaded` has already fired
  focusOnFirstInputElement(); 
}
```


### Additional Properties
cannotChangeDevice
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
        "src": "functions.svg",
        "url": "disableCancel",
        "data": "{{local.dwn1iaw8hl.payload.output.disableCancel}}",
        "tooltip": "{{local.dwn1iaw8hl.payload.output.disableCancel}}",
        "children": [
          {
            "text": "disableCancel"
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


disableCancel
```json 
[
  {
    "children": [
      {
        "text": "true"
      }
    ]
  }
]
```


email
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
        "src": "functions.svg",
        "url": "maskedEmail",
        "data": "{{local.o3p0lu1ww2.payload.output.maskedEmail}}",
        "tooltip": "{{local.o3p0lu1ww2.payload.output.maskedEmail}}",
        "children": [
          {
            "text": "maskedEmail"
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
```
```


inputSchema
```json 
{
    "type": "object",
    "properties": {
         "disableCancel": {
            "displayName": "Disable Cancel Button",
            "preferedControlType": "textField",
            "enableParameters": true
        }
    }
}
```


isEmailDevice
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
        "src": "auth.svg",
        "url": "ciam_allowOnlyEmail",
        "data": "{{global.parameters.ciam_allowOnlyEmail}}",
        "tooltip": "{{global.parameters.ciam_allowOnlyEmail}}",
        "children": [
          {
            "text": "ciam_allowOnlyEmail"
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


maskedEmail
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
        "src": "functions.svg",
        "url": "maskedEmail",
        "data": "{{local.o3p0lu1ww2.payload.output.maskedEmail}}",
        "tooltip": "{{local.o3p0lu1ww2.payload.output.maskedEmail}}",
        "children": [
          {
            "text": "maskedEmail"
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


maskedPhone
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
        "src": "functions.svg",
        "url": "maskedPhone",
        "data": "{{local.o3p0lu1ww2.payload.output.maskedPhone}}",
        "tooltip": "{{local.o3p0lu1ww2.payload.output.maskedPhone}}",
        "children": [
          {
            "text": "maskedPhone"
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


phone
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
        "src": "functions.svg",
        "url": "maskedPhone",
        "data": "{{local.o3p0lu1ww2.payload.output.maskedPhone}}",
        "tooltip": "{{local.o3p0lu1ww2.payload.output.maskedPhone}}",
        "children": [
          {
            "text": "maskedPhone"
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
```
```


validationRules
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [3e3ddhe5la](./3e3ddhe5la.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator |[wb4u3n0g7a](./wb4u3n0g7a.md) | 