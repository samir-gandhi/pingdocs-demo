# Http - Successful user creation
## Configuration
ID:  ak3zkj7i6e

Type: trigger 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | The PingOne user has been successfully created and verified | }
 


## Custom HTML
```html
<div
  class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">
  <div style="max-width: 400px; width: 100%">
    <div class="card shadow mb-5">
      <div class="card-body p-5 d-flex flex-column">
        <img class="companyLogo align-self-center mb-5" alt="{{global.variables.companyName}}" />
        <h1 id="header" class="text-center mb-4">Account Created</h1>
        <p class="text-muted text-center">Your account has been successfully created</p>
        <p class="text-muted text-center">Please click the &#39;Continue&#39; button to Sign On</p>
        <div class="d-flex flex-column">
          <button id="submitBtn" data-id="submitBtn" class="btn btn-primary mb-3" type="submit"
            data-skcomponent="skbutton" data-skbuttontype="next-event" data-skbuttonvalue="Continue">
            Continue
          </button>
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



