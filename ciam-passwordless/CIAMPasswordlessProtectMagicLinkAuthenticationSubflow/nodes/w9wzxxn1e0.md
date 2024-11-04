# Http - string 
Magic Link Form
## Configuration
ID:  w9wzxxn1e0

Type: CONNECTION 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Background Color | html 
#c0dcfdff | 

| Node Description | string 
Request Magic Link | 

## Custom CSS
```css
string 

```

## Custom HTML
```html 
<div
    class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">
    <div class="mh-100" style="max-width: 400px; width: 100%">
        <div class="card shadow mb-5">
            <div class="card-body p-5 d-flex flex-column">
				{{global.parameters.ciam_companyLogo}}
				<p
					class="text-danger mdi mdi-alert-circle"
					data-id="feedback"
					data-skcomponent="skerror">
				</p>
				<p class="text-muted text-center">
					Authenticate by clicking on a link that will be sent to your email address.
				</p>
				<form class="form" id="userSigOnForm" data-id="userSigOnForm">
					<div class="d-flex flex-column mt-5">
						<button id="submit" type="submit" class="btn btn-primary mb-3" data-skcomponent="skbutton"
                            data-skbuttontype="form-submit" data-skform="otp-form" data-skbuttonvalue="submit">
                            Send Link
                        </button>
                        {{#if canChangeDevice}}
                        <button id="cancel" type="button" class="btn btn-link" data-skcomponent="skbutton"
                            data-skbuttontype="next-event" data-skform="otp-form" data-skbuttonvalue="cancel">
                            Cancel
                        </button>
                        {{/if}}
					</div>
				</form>
            </div>
        </div>
    </div>
</div>
```

## Custom Script
```string 

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
        "src": "auth.svg",
        "url": "canChangeDevice",
        "data": "{{global.parameters.canChangeDevice}}",
        "tooltip": "{{global.parameters.canChangeDevice}}",
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
```
```


inputSchema
```json 
{
    "type": "object",
    "properties": {
        "canChangeDevice": {
            "displayName": "more then one usable device",
            "preferedControlType": "textField",
            "enableParameters": true
        }
    }
}
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
| EVAL | [p5i7v1wl02](./p5i7v1wl02.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[m2p5qnib8n](./m2p5qnib8n.md) | 