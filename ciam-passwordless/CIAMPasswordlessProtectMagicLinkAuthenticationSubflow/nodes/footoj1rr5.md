# Http - Success Message
## Configuration
ID:  footoj1rr5

Type: CONNECTION 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Display success message | 
 


## Custom HTML
```html
<div class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">
   <div style="max-width: 400px; min-width: 400px; width: 100%">
        <div class="card shadow mb-5">
            <div class="card-body p-5 d-flex flex-column">
                {{global.parameters.ciam_companyLogo}}
                <h1 class="text-center mb-4">Success</h1>
                <p class="text-muted text-center">You are logged in using a magic link.</p>
                <p class="text-muted text-center">Return to the original window.</p>
                <div class="d-flex flex-column">
                    <!-- <button data-id="button" type="submit" class="btn btn-primary mb-3" data-skcomponent="skbutton"
                            data-skbuttontype="next-event">Exit</button> -->
                            <button type="button" data-id="close-tab" class="btn btn-primary mb-3" data-skcomponent="skbutton" data-skbuttontype="form-submit" data-skform="usernameForm" data-skbuttonvalue="submit"  id="btnClose" >Close current tab</button>
                </div>
            </div>
        </div>
    </div>
</div>
```

## Custom Script
```js
function start() {
    const closeBtn = document.getElementById("btnClose");

    if(closeBtn) {
        closeBtn.addEventListener("click", function(e) {
            // Close the window
            window.close();
            e.preventDefault();
        });
    }

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




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [drn0tajuo1](./drn0tajuo1.md) |  |