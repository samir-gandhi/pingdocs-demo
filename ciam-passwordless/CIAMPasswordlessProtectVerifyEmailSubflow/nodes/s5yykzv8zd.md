# Http - Prompt For Verification Code
## Configuration
ID:  s5yykzv8zd

Type: CONNECTION 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Displays a form for the user to enter the verification code | 
 


## Custom HTML
```html
<div
  class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">
  <div style="max-width: 400px; min-width: 400px; width: 100%">
    <div class="card shadow mb-5">
      <div class="card-body p-5 d-flex flex-column">
        {{global.parameters.ciam_companyLogo}}
        <h1 id="header" class="text-center mb-4">Verification Code</h1>
        <p class="text-muted text-center">
          We’ve sent a verification code to your email address. Verify your email to finish creating your account.
        </p>
        <p id="feedback" data-id="feedback" class="text-danger mdi mdi-alert-circle" data-skcomponent="skerror"></p>
        <p id="verificationCodeFeedback" data-id="verificationCodeFeedback" class="text-danger mdi mdi-alert-circle"
          data-skerrorid="verificationCode" data-skcomponent="skerrormessage"></p>
        <form id="otpForm" data-id="otpForm">
          <div class="mb-4 form-floating">
            <input id="verificationCode" data-id="verificationCode" class="form-control" type="text" name="verificationCode"
              placeholder="Verification Code" autocomplete="off" />
            <label id="verificationCodeLabel" data-id="verificationCodeLabel" class="form-label" for="verificationCode">
              Verification Code
            </label>
          </div>
          <div class="d-flex flex-column">
            <button id="verifyBtn" data-id="verifyBtn" class="btn btn-primary mb-3" type="submit"
              data-skcomponent="skbutton" data-skbuttontype="form-submit" data-skform="otpForm" data-skbuttonvalue="VERIFY">
              Verify
            </button>
            <button type="submit" class="btn btn-link" data-skcomponent="skbutton" data-skbuttontype="next-event" 
              data-skform="otpForm" data-skbuttonvalue="RESEND">
                  Resend verification code
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
  document.getElementById("verificationCode").focus();
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


oeInteractionCacheExpire
 ```json 
false
```


validationRules
 ```json 

```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [qskpbqg2yf](./qskpbqg2yf.md) | [sju60xf677](./sju60xf677.md) |