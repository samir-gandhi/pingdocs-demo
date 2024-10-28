# Http - string 
Password Form
## Configuration
ID:  gnh7rkcsg6

Type: CONNECTION 

CapabilityName: customHTMLTemplate



## Custom HTML
```html 
<div
  class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0">
  <div style="max-width: 400px; width: 100%">
    <div class="card shadow mb-5">
      <div class="card-body p-5 d-flex flex-column">
        {{global.parameters.ciam_companyLogo}}
        <h1 id="header" class="text-center mb-4">Create Your Profile</h1>
        <p id="feedback" data-id="feedback" class="text-danger mdi mdi-alert-circle" data-skcomponent="skerror"></p>
        <form id="registrationForm" data-id="registrationForm" class="form">
          <div id="passwordContainer" class="mb-4 form-floating mt-lg-4">
            <input
              id="password" data-id="password" class="form-control" type="password"
              name="password" placeholder="Password" autocomplete="off" value="" />
            <label class="form-label" for="password">Password</label>
          </div>
          <div id="verifyPasswordContainer" class="mb-4 form-floating">
            <input
              id="verifyPassword" data-id="verifyPassword" class="form-control" type="password"
              name="verifyPassword" placeholder="Verify Password" autocomplete="off" value="" />
            <label class="form-label" for="password">Verify Password</label>
          </div>
          <div class="d-flex flex-column">
            <button id="submitBtn" data-id="submitBtn" class="btn btn-primary mb-3" type="submit" data-skcomponent="skbutton" 
              data-skbuttontype="form-submit" data-skform="registrationForm" data-skbuttonvalue="REGISTER">
                Create Account
            </button>
            <button id="otherBtn" data-id="otherBtn" class="btn btn-link" type="submit" data-skcomponent="skbutton"
                data-skbuttontype="next-event" data-skform="registrationForm" data-skbuttonvalue="OTHER">
                  Sign up without a password
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
  document.getElementById("password").focus();
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
  makePasswordToggle("passwordContainer");
  makePasswordToggle("verifyPasswordContainer");
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
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [tcgo0fso3q](./tcgo0fso3q.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[3os5ylwizz](./3os5ylwizz.md) | 