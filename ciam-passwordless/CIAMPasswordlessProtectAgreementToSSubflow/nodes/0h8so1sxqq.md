# Http - Agreement Form
## Configuration
ID:  0h8so1sxqq

Type: CONNECTION 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Display agreement form to user | 
 


## Custom HTML
```html
<div
    class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0"
>
    <div style="max-width: 400px; width: 100%">
        <div class="card shadow mb-5">
            <div class="card-body p-5 d-flex flex-column">
                {{global.parameters.ciam_companyLogo}}
                <h1 class="text-center mb-4">{{local.8ytvupm9en.payload.output.agreementPresentation.agreementTitle}}</h1>
                <p
                    class="text-danger mdi mdi-alert-circle"
                    data-id="feedback"
                    data-skcomponent="skerror"
                ></p>
                <form id=&#39;agreementForm&#39; data-id="agreementForm">
                    <div class="border overflow-auto mb-4" style="max-height: 300px" data-id="textblock">
                        <div class="p-3" style="white-space: pre-wrap">{{local.8ytvupm9en.payload.output.agreementPresentation.agreementText}}</div>
                    </div>
                    <div class="d-flex flex-column">
                        <button
                            data-id="accept-button"
                            type="submit"
                            data-skcomponent="skbutton"
                            data-skbuttontype="form-submit"
                            data-skform="agreementForm"
                            data-skbuttonvalue="ACCEPT"
                            class="btn btn-primary mb-3"
                        >
                            {{local.8ytvupm9en.payload.output.agreementPresentation.agreementAcceptCheckboxText}}
                        </button>
                        <button
                            data-id="decline-button"
                            type="submit"
                            data-skcomponent="skbutton"
                            data-skbuttontype="form-submit"
                            data-skform="agreementForm"
                            data-skbuttonvalue="DECLINE"
                            class="btn btn-link"
                        >
                            {{local.8ytvupm9en.payload.output.agreementPresentation.agreementDeclineButtonText}}
                        </button>
                    </div>
                </form>
            </div>
        </div>
    </div>
</div>
```


### Additional Properties
formFieldsList
 ```json 

```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [gjg587c8af](./gjg587c8af.md) | [it43isf5sm](./it43isf5sm.md) |