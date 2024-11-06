# Http - string 
Password Form
## Configuration
ID:  1ftyww4qrg

Type: CONNECTION 

CapabilityName: customHTMLTemplate


## Custom CSS
```css
html 
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
[
  {
    "children": [
      {
        "text": "<div  class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0">  <div style="max-width: 400px; width: 100%">    <div class="card shadow mb-5">      <div class="card-body p-5 d-flex flex-column">        "
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "auth.svg",
        "url": "ciam_companyLogo",
        "data": "{{global.parameters.ciam_companyLogo}}",
        "tooltip": "{{global.parameters.ciam_companyLogo}}",
        "children": [
          {
            "text": "{{global.parameters.ciam_companyLogo}}"
          }
        ]
      },
      {
        "text": ""
      },
      {
        "text": "        <h1 id="header" class="text-center mb-4">Create Your Profile</h1>        "
      },
      {
        "text": "<div id="error-wrap">          <p id="feedback" data-id="feedback" class="text-danger mdi mdi-alert-circle" data-skcomponent="skerror"></p>        </div>        <div id="password-error-msg" class="feedback feedback--error sk-alert sk-alert-danger has-text-danger has-background-danger-light password-error"></div>"
      },
      {
        "text": "        <form id="registrationForm" data-id="registrationForm" class="form">          <div id="passwordContainer" class="mb-4 form-floating mt-lg-4">            <input              id="password" data-id="password" class="form-control" type="password"              name="password" placeholder="Password" autocomplete="off" value="" />            <label class="form-label" for="password">Password</label>          </div>          <div id="verifyPasswordContainer" class="mb-4 form-floating">            <input              id="verifyPassword" data-id="verifyPassword" class="form-control" type="password"              name="verifyPassword" placeholder="Verify Password" autocomplete="off" value="" />            <label class="form-label" for="password">Verify Password</label>          </div>          <div class="d-flex flex-column">            <button id="submitBtn" data-id="submitBtn" class="btn btn-primary mb-3" type="submit" data-skcomponent="skbutton"               data-skbuttontype="form-submit" data-skform="registrationForm" data-skbuttonvalue="REGISTER">                Create Account            </button>            <button id="backBtn" data-id="backBtn" class="btn btn-link" type="submit" data-skcomponent="skbutton"                data-skbuttontype="next-event" data-skform="registrationForm" data-skbuttonvalue="BACK">                  Back            </button>            <button id="otherBtn" data-id="otherBtn" class="btn btn-link" type="submit" data-skcomponent="skbutton"                data-skbuttontype="next-event" data-skform="registrationForm" data-skbuttonvalue="OTHER">                  Sign up without a password            </button>          </div>        </form>      </div>    </div>  </div></div>"
      }
    ]
  }
]
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
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [a2zg9lz4ta](./a2zg9lz4ta.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[uf3wbe7ccq](./uf3wbe7ccq.md) | 