# Http - Forgot password form
## Configuration
ID:  qwnvng32z3

Type: trigger 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | A form for the user to submit the username of the account they forgot the password to | }
 


## Custom HTML
```html
[
  {
    "children": [
      {
        "text": ""
      },
      {
        "text": ""
      },
      {
        "text": "<div  class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">  <div style="max-width: 400px; min-width: 400px; width: 100%">    <div class="card shadow mb-5">      <div class="card-body p-5 d-flex flex-column">        <img class="companyLogo align-self-center mb-5" alt=""
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "variable.svg",
        "url": "companyName",
        "data": "{{global.variables.companyName}}",
        "tooltip": "{{global.variables.companyName}}",
        "children": [
          {
            "text": "{{global.variables.companyName}}"
          }
        ]
      },
      {
        "text": ""
      },
      {
        "text": "" />        <h1 id="header" class="text-center mb-4">Password Reset</h1>        <p class="text-muted text-center">          Enter your username, and we&#39;ll send password reset instructions to          your email address.        </p>        <p id="feedback" data-id="feedback" class="text-danger mdi mdi-alert-circle" data-skcomponent="skerror"></p>        <p class="text-danger mdi mdi-alert-circle" data-skerrorid="username" data-skcomponent="skerrormessage"></p>        <form id="usernameForm" data-id="usernameForm">          <div class="mb-4 form-floating">            <input id="username" data-id="username" class="form-control" type="text" name="username"              placeholder="Username" autocomplete="off" value="" />            <label class="form-label" for="email">Username</label>          </div>          <div class="d-flex flex-column">            <button id="submitBtn" data-id="submitBtn" class="btn btn-primary mb-3" type="submit"              data-skcomponent="skbutton" data-skbuttontype="form-submit" data-skform="usernameForm" data-skbuttonvalue="SUBMIT">              Submit            </button>            <button id="cancelBtn" data-id="cancelBtn" class="btn btn-link" type="submit" data-skcomponent="skbutton"              data-skbuttontype="next-event" data-skform="usernameForm" data-skbuttonvalue="CANCEL">              Cancel            </button>          </div>        </form>      </div>    </div>  </div></div>"
      }
    ]
  }
]
```

## Custom Script
```js
const focusOnFirstInputElement = () => {
  document.getElementById("username").focus();
};

/**
 * If page isn&#39;t loaded yet, wait for the page to load, then focus on first
 * input element.
 */
if (document.readyState === "loading") {
  // Loading hasn&#39;t finished yet
  document.onreadystatechange = () => {
    if (document.readyState === "complete") {
      focusOnFirstInputElement();
    }
  };
} else {
  // `DOMContentLoaded` has already fired
  focusOnFirstInputElement();
}

```

### Additional Properties
formFieldsList
 ```json 

```


validationRules
 ```json 

```



