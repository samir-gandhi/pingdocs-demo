# Http - string 
Reset Password Success Message
## Configuration
ID:  se0w7zdrd7

Type: CONNECTION 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
Displays a success page for update password | 


## Custom HTML
```html 
<div
  class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">
  <div style="max-width: 400px; width: 100%">
    <div class="card shadow mb-5">
      <div class="card-body p-5 d-flex flex-column">
        {{local.4rjs3llu20.payload.output.flowCompanyLogo}}
        <h1 id="header" class="text-center mb-4">Success</h1>
        <p class="text-muted text-center">
          Your password has been updated.
        </p>
        <form id="authForm" data-id="authForm">
					<div class="d-flex flex-column mt-5">
            <button id="submitBtn" data-id="submitBtn" class="btn btn-primary mb-3" type="submit"
              data-skcomponent="skbutton" data-skbuttontype="form-submit" data-skform="form" data-skbuttonvalue="CONTINUE">
              Next
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





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [8b7afymuxh](./8b7afymuxh.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[liu3llworn](./liu3llworn.md) | 