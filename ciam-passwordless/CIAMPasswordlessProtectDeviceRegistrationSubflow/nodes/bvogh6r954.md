# Http - string 
Email Form
## Configuration
ID:  bvogh6r954

Type: CONNECTION 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
User enters email | 


## Custom HTML
```html 
<div
  class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">
  <div class="mh-100" style="max-width: 400px; width: 100%;">
    <div class="card shadow mb-5">
      <div class="card-body p-5 d-flex flex-column">
        {{global.parameters.ciam_companyLogo}}
        <h1 class="text-center mb-4">
            <i class="mdi mdi-email-outline text-dark fs-2" aria-hidden="true"></i>
            Email Address
        </h1>
        <p class="text-muted text-center">
            Enter the email address that you want to use for authentication.
        </p>
        <p id="feedback" data-id="feedback" class="text-danger mdi mdi-alert-circle" data-skcomponent="skerror"></p>
        <p class="text-danger mdi mdi-alert-circle" data-skerrorid="email" data-skcomponent="skerrormessage"></p>
        <form id="emailForm" data-id="emailForm">
          <div class="mb-4 form-floating">
            <input id="email" data-id="email" class="form-control" type="text" name="email" placeholder="Email Address" autocomplete="off" />
            <label id="emailLabel" data-id="emailLabel" class="form-label" for="email">Email Address</label>
          </div>
          <div class="d-flex flex-column">
              <button id="submit" class="btn btn-primary mb-3" data-skcomponent="skbutton"
                  data-skbuttontype="form-submit" data-skform="emailForm" data-skbuttonvalue="submit">
                  Next
              </button>
              <button id="cancel" class="btn btn-link" data-skcomponent="skbutton"
                  data-skbuttontype="next-event" data-skform="emailForm" data-skbuttonvalue="cancel">
                  Cancel
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
```
```


validationRules
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [4smjdpxvyk](./4smjdpxvyk.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[rkuiz7q78p](./rkuiz7q78p.md) | 