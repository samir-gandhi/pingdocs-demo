# Http - Forgot password recovery code form
## Configuration
ID:  fkekf3oi8e

Type: trigger 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | A form to enter the password recovery code and a new password | }
 


## Custom HTML
```html
<div
  class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">
  <div style="max-width: 400px; min-width: 400px; width: 100%">
    <div class="card shadow mb-5">
      <div class="card-body p-5 d-flex flex-column">
        <img class="companyLogo align-self-center mb-5" alt="{{global.variables.companyName}}" />
        <h1 id="header" class="text-center mb-4">Enter New Password</h1>
        <p class="text-muted text-center">
          If you have an active account with a valid email address, you will
          receive an email with a recovery code which you may enter here, along
          with a new password.
        </p>
        <p class="text-muted text-center">
          If you do not have an account or email, please contact your
          administrator to recover your password.
        </p>
        <p id="feedback" data-id="feedback" class="text-danger mdi mdi-alert-circle" data-skcomponent="skerror"></p>
        <form id="recoveryCodeForm" data-id="recoveryCodeForm">
          <div class="mb-4 form-floating">
            <input id="recoveryCode" data-id="recoveryCode" class="form-control" type="text" name="recoveryCode"
              placeholder="Recovery Code" autocomplete="on" value=""/>
            <label id="recoveryCodeLabel" data-id="recoveryCodeLabel" class="form-label" for="recoveryCode">
              Recovery Code
            </label>
          </div>
          <div id="newPasswordContainer" class="mb-4 form-floating">
            <input id="newPassword" data-id="newPassword" class="form-control" type="password" name="newPassword"
              placeholder="New Password" autocomplete="on" value="" />
            <label id="newPasswordLabel" data-id="newPasswordLabel" class="form-label" for="newPassword" >
              New Password
            </label>
          </div>
          <div class="d-flex flex-column">
            <button id="submitBtn" data-id="submitBtn" class="btn btn-primary mb-3" type="submit" data-skcomponent="skbutton"
              data-skbuttontype="form-submit" data-skform="recoveryCodeForm" data-skbuttonvalue="SUBMIT" >
              Submit
            </button>
            <button id="cancelBtn" data-id="cancelBtn" class="btn btn-link" type="submit" data-skcomponent="skbutton"
              data-skbuttontype="next-event" data-skform="recoveryCodeForm" data-skbuttonvalue="CANCEL">
              Cancel
            </button>
          </div>
        </form>
      </div>
    </div>
  </div>
</div>
```

## Custom Script
```js
const focusOnFirstInputElement = () => {
  document.getElementById("recoveryCode").focus();
};

function makePasswordToggle(id) {
    var container = document.getElementById(id);
    var password = container.getElementsByTagName("input")[0];
    var toggler = document.createElement("button");
    toggler.setAttribute("type", "button");
    toggler.setAttribute("aria-label", "Show/Hide Password");
    toggler.className = "btn mdi mdi-eye-off-outline position-absolute end-0 top-50 translate-middle-y";
    container.appendChild(toggler);

    function showHidePassword() {
        if (password.type == "password") {
            password.setAttribute("type", "text");
            toggler.classList.add("mdi-eye-outline");
            toggler.classList.remove("mdi-eye-off-outline");
        } else {
            toggler.classList.add("mdi-eye-off-outline");
            toggler.classList.remove("mdi-eye-outline");
            password.setAttribute("type", "password");
        }
        password.focus();
    };

    toggler.addEventListener("click", showHidePassword);
}

function start() {
    makePasswordToggle("newPasswordContainer");
    focusOnFirstInputElement();
}

if (document.readyState === "loading") {
    // Loading hasn&#39;t finished yet
    document.addEventListener("DOMContentLoaded", start);
} else {
    // `DOMContentLoaded` has already fired
    start();
}
```

### Additional Properties
formFieldsList
 ```json 

```


nextButtonText
 ```json 
Sign On
```


title
 ```json 
Recover Password
```


validationRules
 ```json 

```



