# Http - string 
Display User Devices
## Configuration
ID:  kdfb05yf1m

Type: CONNECTION 

CapabilityName: customHTMLTemplate


## Custom CSS
```css
json 
[id^="mfa-type-list-button"] div {
    flex: 1;
}
```

## Custom HTML
```html 
<div
    class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">
    <div class="mh-100" style="max-width: 400px; width: 100%;">
        <div class="card shadow mb-5">
            <div class="card-body p-5 d-flex flex-column">
                <div class="dialog-content-header dialog-content__header" style="height: 50px">
                    <div class="dialog-content-header__logo"></div>
                </div>
            </div>
                <h1 class="text-center mb-4">Your authentication methods</h1>
                {{#if successMessage}}
                <p id="successMessage" style="display: flex" class="text-success mdi mdi-check-circle my-4">{{successMessage}}</p>
                {{/if}}
                {{#if deviceRemovalWarning}}
                <p class="text-warning mdi mdi-alert-circle my-4">
                    Removing all authentication methods could prevent you from signing  on to your account.
                </p>
                {{/if}}
                <p class="text-danger mdi mdi-alert-circle my-4" data-id="feedback" data-skcomponent="skerror"></p>
                <form id="authentication-methods" data-id="authentication-methods">
                    <div class="d-flex flex-column gap-4 mb-4">
                        {{#each devices}}
                        {{#ifEquals type "SMS"}}
                        <button class="btn btn-outline-light flex-grow-1 d-flex align-items-center gap-4"
                            id="mfa-type-list-button-SMS-{{id}}" data-skcomponent="skbutton"
                            data-skbuttontype="next-event" data-skbuttonvalue="{{id}}">
                            <div class="flex-grow-1 d-flex align-items-center gap-4">
                                <i class="mdi mdi-comment-text-outline text-dark fs-2" aria-hidden="true"></i>
                                <div class="d-flex flex-column text-start gap-1">
                                    <div class="fw-semibold text-primary">
                                        {{#if nickname}}
                                            {{nickname}}
                                        {{else}}
                                            Text Message
                                        {{/if}}
                                    </div>
                                    <div class="fs-5 text-secondary text-break">
                                        {{phone}}
                                    </div>
                                </div>
                                {{#if @first}} <span class="text-muted">Default</span> {{/if}}
                            </div>
                        </button>
                        {{/ifEquals}}
                        {{#ifEquals type "EMAIL"}}
                        <button class="btn btn-outline-light flex-grow-1 d-flex align-items-center gap-4"
                            id="mfa-type-list-button-EMAIL-{{id}}" data-skcomponent="skbutton"
                            data-skbuttontype="next-event" data-skbuttonvalue="{{id}}">
                            <div class="flex-grow-1 d-flex align-items-center gap-4">
                                <i class="mdi mdi-email-outline text-dark fs-2" aria-hidden="true"></i>
                                <div class="d-flex flex-column text-start gap-1">
                                    <div class="fw-semibold text-primary">
                                        {{#if nickname}}
                                            {{nickname}}
                                        {{else}}
                                            Email
                                        {{/if}}
                                    </div>
                                    <div class="fs-5 text-secondary text-break">
                                        {{email}}
                                    </div>
                                </div>
                                {{#if @first}} <span class="text-muted">Default</span> {{/if}}
                            </div>
                        </button>
                        {{/ifEquals}}
                        {{#ifEquals type "FIDO2"}}
                        <button class="btn btn-outline-light flex-grow-1 d-flex align-items-center gap-4"
                            id="mfa-type-list-button-FIDO2-{{id}}" data-skcomponent="skbutton"
                            data-skbuttontype="next-event" data-skbuttonvalue="{{id}}">
                            <div class="flex-grow-1 d-flex align-items-center gap-4">
                                <svg viewBox="0 0 27 26" role="presentation" style="width: 20px; height: 20px;">
                                    <path d="M10.2632 12.3158C13.6641 12.3158 16.4211 9.55881 16.4211 6.15789C16.4211 2.75698 13.6641 0 10.2632 0C6.86225 0 4.10527 2.75698 4.10527 6.15789C4.10527 9.55881 6.86225 12.3158 10.2632 12.3158Z" fill="#3D454D" />
                                    <path d="M26.6842 12.3158C26.6842 9.67474 24.5631 7.51263 21.9084 7.51263C19.2674 7.51263 17.1053 9.63369 17.1053 12.2884C17.1053 14.1495 18.1589 15.8326 19.8421 16.6263V23.9474L21.8947 26L25.3158 22.5789L23.2631 20.5263L25.3158 18.4737L23.6189 16.7768C25.4663 16.0653 26.6842 14.2863 26.6842 12.3158ZM21.8947 12.3158C21.1421 12.3158 20.5263 11.7 20.5263 10.9474C20.5263 10.1947 21.1421 9.57895 21.8947 9.57895C22.6474 9.57895 23.2631 10.1947 23.2631 10.9474C23.2631 11.7 22.6474 12.3158 21.8947 12.3158Z" fill="#3D454D" />
                                    <path d="M15.6547 15.08C14.6011 14.6147 13.4653 14.3684 12.3158 14.3684H8.21053C3.68105 14.3684 0 18.0495 0 22.5789V25.3158H17.7895V17.7758C16.8726 17.0642 16.1337 16.1474 15.6547 15.08Z" fill="#3D454D" />
                                </svg>
                                <div class="d-flex flex-column text-start gap-1">
                                    {{#if nickname}}
                                        <div class="fw-semibold text-primary">
                                            {{nickname}}
                                        </div>
                                    {{else}}
                                        <div class="fw-semibold text-primary">
                                            Biometrics/Security Key
                                        </div>
                                    {{/if}}
                                </div>
                                {{#if @first}} <span class="text-muted">Default</span> {{/if}}
                            </div>
                        </button>
                        {{/ifEquals}}
                        {{/each}}
                    </div>
                    <div class="d-flex flex-column">
                        {{#if canAddNewMethod}}
                        <button type="submit" class="btn btn-link mb-3" data-skcomponent="skbutton"
                            data-skbuttontype="next-event" data-skform="authentication-methods" data-skbuttonvalue="ADD"
                            id="add">
                            &#43; Add method
                        </button>
                        {{/if}}
                        {{#unless successMessage}}
                        <button id="cancelBtn" data-id="cancelBtn" class="btn btn-link mb-3" type="submit" data-skcomponent="skbutton"
                            data-skbuttontype="next-event" data-skform="authentication-methods" data-skbuttonvalue="CANCEL">
                            Cancel
                        </button>
                        {{else}}
                        <button id="doneBtn" data-id="doneBtn" class="btn btn-outline-primary mb-3" type="submit" data-skcomponent="skbutton"
                            data-skbuttontype="next-event" data-skform="authentication-methods" data-skbuttonvalue="DONE">
                            Done
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
document.onclick = function(e) {
  const divToHide = document.getElementById("successMessage")
  if (divToHide != null) {
    divToHide.style.display = "none";
  }
}

```


### Additional Properties
canAddNewMethod
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
        "url": "success",
        "data": "{{local.lxdqcv1aa7.payload.success}}",
        "tooltip": "{{local.lxdqcv1aa7.payload.success}}",
        "children": [
          {
            "text": "success"
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


deviceRemovalWarning
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
        "url": "deviceRemovalWarning",
        "data": "{{local.8sttri4np9.payload.output.deviceRemovalWarning}}",
        "tooltip": "{{local.8sttri4np9.payload.output.deviceRemovalWarning}}",
        "children": [
          {
            "text": "deviceRemovalWarning"
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


devices
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
        "url": "usableDevices",
        "data": "{{local.pks46w5ks6.payload.output.usableDevices}}",
        "tooltip": "{{local.pks46w5ks6.payload.output.usableDevices}}",
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
		"devices":{
			"type":"array"
		},
		"canAddNewMethod":{
			"type":"boolean"
		},
		"successMessage":{
			"type":"string"
		},
		"deviceRemovalWarning":{
			"type":"boolean"
		}
	}
}
```


successMessage
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
        "url": "successMessage",
        "data": "{{local.9pekqghawg.payload.output.successMessage}}",
        "tooltip": "{{local.9pekqghawg.payload.output.successMessage}}",
        "children": [
          {
            "text": "successMessage"
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
| EVAL | [4wqs0nbs1v](./4wqs0nbs1v.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[0jgff1lx32](./0jgff1lx32.md) | 