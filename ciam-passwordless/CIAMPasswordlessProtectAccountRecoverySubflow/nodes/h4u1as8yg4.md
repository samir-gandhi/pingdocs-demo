# Http - Recovery Code Form
## Configuration
ID:  h4u1as8yg4

Type: CONNECTION 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | A form to enter the password recovery code and a new password | 
 

## Custom CSS
```css
.input-policy-error {
    margin-top: 0rem;
    text-align: left;
    margin-left: 0rem;
    margin-bottom: 1rem;
    line-height: 1.5;
    color: #a61908;
}
```

## Custom HTML
```html
<div
  class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">
  <div style="max-width: 400px; min-width: 400px; width: 100%">
    <div class="card shadow mb-5">
      <div class="card-body p-5 d-flex flex-column">
        {{global.parameters.ciam_companyLogo}}
        <h1 id="header" class="text-center mb-4">Enter New Password</h1>
        <p class="text-muted text-center">
          An email with a recovery code has been sent to your email address.
        </p>
        <div id="error-wrap">
          <p id="feedback" data-id="feedback" class="text-danger mdi mdi-alert-circle" data-skcomponent="skerror"></p>
        </div>
        <div id="password-error-msg" class="feedback feedback--error sk-alert sk-alert-danger has-text-danger has-background-danger-light password-error"></div>
        <p class="text-danger mdi mdi-alert-circle" data-skerrorid="recoveryCode" data-skcomponent="skerrormessage"></p>
        <p class="text-danger mdi mdi-alert-circle" data-skerrorid="newPassword" data-skcomponent="skerrormessage"></p>
        <p class="text-danger mdi mdi-alert-circle" data-skerrorid="verifyNewPassword" data-skcomponent="skerrormessage"></p>
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
          <div id="verifyPasswordContainer" class="mb-4 form-floating">
            <input
              id="verifyNewPassword" data-id="verifyNewPassword" class="form-control" type="password"
              name="verifyNewPassword" placeholder="Verify New Password" autocomplete="off" value="" />
            <label class="form-label" for="email">Verify New Password</label>
          </div>
          <div class="d-flex flex-column">
            <button id="resendBtn" type="resendBtn" class="btn btn-link" data-skcomponent="skbutton" style="margin-bottom: 15px;"
              data-skbuttontype="next-event" data-skbuttonvalue="RESEND">
              Resend recovery code
            </button>
          </div>
          <div class="d-flex flex-column">
            <button id="submitBtn" data-id="submitBtn" class="btn btn-primary mb-3" type="submit" data-skcomponent="skbutton"
              data-skbuttontype="form-submit" data-skform="recoveryCodeForm" data-skbuttonvalue="SUBMIT" >
              Submit
            </button>
            <button id="backBtn" data-id="backBtn" class="btn btn-link" type="submit" data-skcomponent="skbutton"
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

var errorDiv = document.getElementById(&#39;error-wrap&#39;);
if(window.addEventListener) {
   // Normal browsers
   errorDiv.addEventListener(&#39;DOMSubtreeModified&#39;, contentChanged, false);
} else if(window.attachEvent) {
    // IE
    errorDiv.attachEvent(&#39;DOMSubtreeModified&#39;, contentChanged);
}

// Maps the password policy requirements to well-formed messages
function contentChanged() {
   let errorMsg  = document.getElementById(&#39;feedback&#39;);
   let passwordErrorMsg  = document.getElementById(&#39;password-error-msg&#39;);
   passwordErrorMsg.innerText = "";

   if (errorMsg) {
       if (errorMsg.innerText.includes("passwordPolicies:")) {
          const policies = [];
          let textNode = document.createTextNode("Your password must:");
          passwordErrorMsg.appendChild(textNode);
          
          if (errorMsg.innerText.includes("minCharactersLowercase")) {
            policies.push("Contain at least 1 lowercase letter.");
          }
          if (errorMsg.innerText.includes("minCharactersUppercase")) {
            policies.push("Contain at least 1 uppercase letter.");
          }
          if (errorMsg.innerText.includes("minCharactersSpecialChar")) {
            policies.push("Contain at least 1 of these special characters: ~!@#$%^&amp;*()-_=&#43;[]{}|;:,.<>/?");
          }
          if (errorMsg.innerText.includes("minCharactersNumeric")) {
            policies.push("Contain at least 1 number.");
          }
          if (errorMsg.innerText.includes("minUniqueCharacters")) {
            policies.push("Include at least 5 unique characters.");
          }
          if (errorMsg.innerText.includes("excludesCommonlyUsed")) {
            policies.push("Not be on the list of the most commonly-used passwords.");
          }
          if (errorMsg.innerText.includes("passwordPolicies:The provided new password cannot be the same as the current password or any password in the user&#39;s password history.")) {
            policies.push("The provided new password cannot be the same as the current password or any password from your password history.");
          }
          if (errorMsg.innerText.includes("maxRepeatedCharacters")) {
            policies.push("Not have more than 2 of the same characters in a row. For example, &#39;aa&#39; is acceptable but &#39;aaa&#39; is not.");
          }
          if (errorMsg.innerText.includes("length")) {
            // Handles parsing the length requirement in the event the length is double digits. Will need to update this if length is 3 digits. Highly uncommon.
            const errorMessage = errorMsg.innerText;
            const index = errorMessage.indexOf("length");
            if (index !== -1 &amp;&amp; index < errorMessage.length - 1) {
  					  let length = errorMessage[index &#43; 6];
              if (errorMessage[index &#43; 7] !== " " &amp;&amp; errorMessage[index &#43; 7] !== undefined) {
                length = length &#43; errorMessage[index &#43; 7];
              }
              policies.push("Be at least " &#43; length &#43; " characters long.");
					  }
          }

          if(policies.length === 0) policies.push("Follow password policy requirements.");

          policies.forEach(policy => {
            const li = document.createElement("li");
            li.textContent = policy;
            passwordErrorMsg.appendChild(li);
          });
            passwordErrorMsg.classList.add("input-policy-error");
            errorMsg.style.display = "none";
        } else {
            // leave message as-is
        }
   }
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




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [zvl6xidgq9](./zvl6xidgq9.md) | [n9tgrbpiz4](./n9tgrbpiz4.md) |