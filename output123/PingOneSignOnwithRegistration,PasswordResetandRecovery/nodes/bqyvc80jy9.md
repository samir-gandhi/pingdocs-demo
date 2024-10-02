# Http - Success Message
## Configuration
ID:  bqyvc80jy9

Type: trigger 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Display success message | }
 


## Custom HTML
```html
<div class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">
   <div style="max-width: 400px; min-width: 400px; width: 100%">
        <div class="card shadow mb-5">
            <div class="card-body p-5 d-flex flex-column">
                <img class="companyLogo align-self-center mb-5" alt="{{global.variables.companyName}}" />
                <h1 class="text-center mb-4">Success</h1>
                <p class="text-muted text-center">Your password has been successfully updated.</p>
                <div class="d-flex flex-column">
                    <button data-id="button" type="submit" class="btn btn-primary mb-3" data-skcomponent="skbutton"
                            data-skbuttontype="next-event">Continue</button>
                </div>
            </div>
        </div>
    </div>
</div>
```


### Additional Properties
formFieldsList
 ```json 

```



