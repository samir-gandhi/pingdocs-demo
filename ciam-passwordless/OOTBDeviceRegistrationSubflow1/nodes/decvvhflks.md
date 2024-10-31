# Http - string 
Display Device Types
## Configuration
ID:  decvvhflks

Type: CONNECTION 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
Display available methods | 

## Custom CSS
```css
string 

```

## Custom HTML
```html 
<div
    class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">
    <div class="mh-100" style="max-width: 400px; width: 100%;">
        <div class="card shadow mb-5">
            <div class="card-body p-5 d-flex flex-column">
                {{global.parameters.ciam_companyLogo}}
                <h1 class="text-center mb-4">Select Method</h1>
                <p class="text-muted text-center">
                    Select the authentication method you want to pair with your account
                </p>
                <form id="method-selection" data-id="method-selection">
                    <div class="d-flex flex-column gap-4 mb-4">
                        {{#each allowedTypes as | type |}}
                        {{#ifEquals type "FIDO2"}}
                        <button class="btn btn-outline-light flex-grow-1 d-flex align-items-center gap-4"
                            id="mfa-type-list-button-FIDO2" data-skcomponent="skbutton"
                            data-skbuttontype="next-event" data-skbuttonvalue="FIDO2">
                            <div class="flex-grow-1 d-flex align-items-center gap-4">
                                 <svg viewBox="0 0 27 26" role="presentation" style="width: 20px; height: 20px;">
                                    <path d="M10.2632 12.3158C13.6641 12.3158 16.4211 9.55881 16.4211 6.15789C16.4211 2.75698 13.6641 0 10.2632 0C6.86225 0 4.10527 2.75698 4.10527 6.15789C4.10527 9.55881 6.86225 12.3158 10.2632 12.3158Z" fill="#3D454D" />
                                    <path d="M26.6842 12.3158C26.6842 9.67474 24.5631 7.51263 21.9084 7.51263C19.2674 7.51263 17.1053 9.63369 17.1053 12.2884C17.1053 14.1495 18.1589 15.8326 19.8421 16.6263V23.9474L21.8947 26L25.3158 22.5789L23.2631 20.5263L25.3158 18.4737L23.6189 16.7768C25.4663 16.0653 26.6842 14.2863 26.6842 12.3158ZM21.8947 12.3158C21.1421 12.3158 20.5263 11.7 20.5263 10.9474C20.5263 10.1947 21.1421 9.57895 21.8947 9.57895C22.6474 9.57895 23.2631 10.1947 23.2631 10.9474C23.2631 11.7 22.6474 12.3158 21.8947 12.3158Z" fill="#3D454D" />
                                    <path d="M15.6547 15.08C14.6011 14.6147 13.4653 14.3684 12.3158 14.3684H8.21053C3.68105 14.3684 0 18.0495 0 22.5789V25.3158H17.7895V17.7758C16.8726 17.0642 16.1337 16.1474 15.6547 15.08Z" fill="#3D454D" />
                                </svg>
                                <div class="d-flex flex-column text-start gap-1">
                                    <div class="fw-semibold text-primary">
                                        Biometrics/Security Key
                                    </div>
                                    <div class="fs-5 text-secondary">
                                        Use Biometrics/Security Key to authenticate.
                                    </div>
                                </div>
                            </div>
                        </button>
                        {{/ifEquals}} 
                        {{#ifEquals type "SMS"}}
                        <button class="btn btn-outline-light flex-grow-1 d-flex align-items-center gap-4"
                            id="mfa-type-list-button-SMS" data-skcomponent="skbutton" data-skbuttontype="next-event"
                            data-skbuttonvalue="SMS">
                            <div class="flex-grow-1 d-flex align-items-center gap-4">
                                <i class="mdi mdi-comment-text-outline text-dark fs-2" aria-hidden="true"></i>
                                <div class="d-flex flex-column text-start gap-1">
                                    <div class="fw-semibold text-primary">
                                        Text Message
                                    </div>
                                    <div class="fs-5 text-secondary">
                                        Receive a text message with a passcode to authenticate.
                                    </div>
                                </div>
                            </div>
                        </button>
                        {{/ifEquals}}
                        {{#ifEquals type "EMAIL"}}
                        <button class="btn btn-outline-light flex-grow-1 d-flex align-items-center gap-4"
                            id="mfa-type-list-button-EMAIL" data-skcomponent="skbutton" data-skbuttontype="next-event"
                            data-skbuttonvalue="EMAIL">
                            <div class="flex-grow-1 d-flex align-items-center gap-4">
                                <i class="mdi mdi-email-outline text-dark fs-2" aria-hidden="true"></i>
                                <div class="d-flex flex-column text-start gap-1">
                                    <div class="fw-semibold text-primary">
                                        Email
                                    </div>
                                    <div class="fs-5 text-secondary">
                                        Receive an email with a passcode to authenticate.
                                    </div>
                                </div>
                            </div>
                        </button>
                        {{/ifEquals}}
                        {{/each}}
                    </div>
                    {{#unless passwordlessRequired}}
                    <div class="d-flex flex-column">
                        <button class="btn btn-link mb-3" 
                            id="mfa-type-list-button-PASSWORD" data-skcomponent="skbutton"
                            data-skbuttontype="next-event" data-skbuttonvalue="PASSWORD">
                            Register with password 
                        </button>
                    </div>
                    {{/unless}}
                    {{#if allowCancel}}
                    <div class="d-flex flex-column">
                        <button class="btn btn-link mb-3" 
                            id="mfa-type-list-button-CANCEL" data-skcomponent="skbutton"
                            data-skbuttontype="next-event" data-skbuttonvalue="CANCEL">
                            Cancel
                        </button>
                    </div>
                    {{/if}}
                </form>
            </div>
        </div>
    </div>
</div>
```

## Custom Script
```string 

```

### Output Schema
``` json 
{
	"type": "object",
	"properties": {
		"buttonValue": {
			"type": "string",
			"propertyName": "buttonValue"
		}
	}
} 
```

### Additional Properties
allowCancel
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
        "url": "allowCancel",
        "data": "{{global.parameters.allowCancel}}",
        "tooltip": "{{global.parameters.allowCancel}}",
        "children": [
          {
            "text": "allowCancel"
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


allowedTypes
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
        "url": "usableDevices",
        "data": "{{local.wc0jfkkr3z.payload.output.usableDevices}}",
        "tooltip": "{{local.wc0jfkkr3z.payload.output.usableDevices}}",
        "children": [
          {
            "text": "usableDevices"
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
		"allowedTypes": {
			"type": "array"
		},
		"passwordlessRequired": {
			"type": "boolean"
		},
		"allowCancel": {
			"type": "boolean"
		}
	}
}
```


messageTitle
```json 
[
  {
    "children": [
      {
        "text": "Information"
      }
    ]
  }
]
```


passwordlessRequired
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
        "url": "passwordlessRequired",
        "data": "{{global.parameters.passwordlessRequired}}",
        "tooltip": "{{global.parameters.passwordlessRequired}}",
        "children": [
          {
            "text": "passwordlessRequired"
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


typeDisplayNames
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
        "url": "typeDisplayNames",
        "data": "{{local.wc0jfkkr3z.payload.output.typeDisplayNames}}",
        "tooltip": "{{local.wc0jfkkr3z.payload.output.typeDisplayNames}}",
        "children": [
          {
            "text": "typeDisplayNames"
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
| EVAL | [zurglr5j5k](./zurglr5j5k.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[k44ne8uadp](./k44ne8uadp.md) | 