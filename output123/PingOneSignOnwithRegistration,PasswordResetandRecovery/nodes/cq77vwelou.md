# Http - Username/Password Form
## Configuration
ID:  cq77vwelou

Type: trigger 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Background Color | #afd5ffff | 

 


## Custom HTML
```html
<div
    class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">
    <div style="max-width: 400px; min-width: 400px; width: 100%">
        <div class="card shadow mb-5">
            <div class="card-body p-5 d-flex flex-column">
                <img class="companyLogo align-self-center mb-5" alt="{{global.variables.companyName}}" />
                <h1 class="text-center mb-4">Sign On</h1>
                <p class="text-muted text-center">Welcome to Ping Identity</p>
                <p class="text-danger mdi mdi-alert-circle" data-id="feedback" data-skcomponent="skerror"></p>
                <form id="usernamePasswordForm" data-id="usernamePasswordForm">
                    <div class="mb-4 form-floating">
                        <input class="form-control" type="text" id="username" name="username" placeholder="username"
                            autocomplete="off" value="" data-id="username-input" />
                        <label class="form-label" for="username">Username</label>
                    </div>
                    <div id="passwordContainer" class="mb-4 form-floating">
                        <input class="form-control" type="password" id="password" name="password" placeholder="Password"
                            autocomplete="off" value="" data-id="password-input" />
                        <label class="form-label" for="password">Password</label>
                    </div>
                    <div class="d-flex flex-column">
                        <button data-id="button" type="submit" class="btn btn-primary mb-3" data-skcomponent="skbutton"
                            data-skbuttontype="form-submit" data-skform="usernamePasswordForm" id="btnSignIn"
                            data-skbuttonvalue="SIGNON">
                            Sign On
                        </button>
                        <div class="d-flex flex-column">
                            <button data-id="button" type="submit" class="btn btn-link" data-skcomponent="skbutton"
                                data-skbuttontype="form-submit" data-skform="usernamePasswordForm" id="btnTrouble"
                                data-skbuttonvalue="TROUBLE">
                                Having trouble signing on?
                            </button>
                            <button data-id="button" type="submit" class="btn btn-link" data-skcomponent="skbutton"
                                data-skbuttontype="next-event" data-skform="usernamePasswordForm" id="btnRegister"
                                data-skbuttonvalue="REGISTER">
                                No account? Register now!
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
    document.getElementById("username").focus();
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


inputSchema
 ```json 

```


validationRules
 ```json 

```



