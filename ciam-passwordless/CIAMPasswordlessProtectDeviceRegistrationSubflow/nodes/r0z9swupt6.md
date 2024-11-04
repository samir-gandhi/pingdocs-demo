# Http - string 
Phone Number Form
## Configuration
ID:  r0z9swupt6

Type: CONNECTION 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
User enters phone number | 


## Custom HTML
```html 
<div
    class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">
    <div class="mh-100" style="max-width: 400px; width: 100%;">
        <div class="card shadow mb-5">
            <div class="card-body p-5 d-flex flex-column">
                {{global.parameters.ciam_companyLogo}}
                <h1 class="text-center mb-4">
                    <i class="mdi mdi-comment-text-outline text-dark fs-1" aria-hidden="true"></i>
                    Text Message
                </h1>
                <p class="text-muted text-center">
                    Enter the phone number including the country code that you want to use for authentication.
                </p>
                <p class="text-danger mdi mdi-alert-circle" data-id="feedback" data-skcomponent="skerror"></p>
                <p class="text-danger mdi mdi-alert-circle" data-skerrorid="phone" data-skcomponent="skerrormessage"></p>
                <form id="phone-form" data-id="phone-form">
                    <div class="mb-4 form-floating">
                        <input id="phone" data-id="phone" class="form-control" type="text" name="phone" placeholder="Phone Number" autocomplete="off"/>
                        <label id="phoneLabel" data-id="phoneLabel" class="form-label" for="phone">Phone Number</label>
                    </div>
                    <div class="d-flex flex-column">
                        <button id="submit" class="btn btn-primary mb-3" data-skcomponent="skbutton"
                            data-skbuttontype="form-submit" data-skform="phone-form" data-skbuttonvalue="submit">
                            Next
                        </button>
                        <button id="cancel" class="btn btn-link" data-skcomponent="skbutton"
                            data-skbuttontype="next-event" data-skform="phone-form" data-skbuttonvalue="cancel">
                            Cancel
                        </button>
                    </div>
                </form>
                <p class="text-muted text-center mt-3">I agree to receive a one-time passcode. Message and data rates may
                    apply. Reply STOP to unsubscribe.
                </p>
            </div>
        </div>
    </div>
</div>
```


### Output Schema
``` json 
{
	"type": "object",
	"properties": {
		"buttonValue": {
			"type": "string",
			"propertyName": "buttonValue"
		},
		"phone": {
			"type": "string",
			"propertyName": "phone"
		},
		"countryCode": {
			"type": "string",
			"propertyName": "countryCode"
		}
	}
} 
```

### Additional Properties
formFieldsList
```
```


validationRules
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [ocsgnkoz0e](./ocsgnkoz0e.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[0s68cax470](./0s68cax470.md) | 