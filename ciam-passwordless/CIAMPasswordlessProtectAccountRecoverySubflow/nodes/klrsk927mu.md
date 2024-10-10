# Http - Forgot Password Form
## Configuration
ID:  klrsk927mu

Type: CONNECTION 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | A form for the user to submit the email of the account they forgot the password to | 
 


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
        "type": "link",
        "data": "[[[skcomponent###c2tjb21wb25lbnQgInNrcmlzayIgIGVudmlyb25tZW50SWQ9IiIgY29sbGVjdEJlaGF2aW9yYWxEYXRhPSJ0cnVlIiBwcm9wZXJ0eW5hbWU9InJpc2tmcCI=###eyJuYW1lIjoic2tyaXNrIiwib3B0aW9ucyI6eyJlbnZpcm9ubWVudElkIjoiIiwiY29sbGVjdEJlaGF2aW9yYWxEYXRhIjoidHJ1ZSIsInByb3BlcnR5bmFtZSI6InJpc2tmcCJ9LCJjb21wb25lbnRQcm9wcyI6eyJlbnZpcm9ubWVudElkIjp7Im5hbWUiOiJlbnZpcm9ubWVudElkIiwiZGlzcGxheU5hbWUiOiJFbnZpcm9ubWVudCBJRCJ9LCJjb2xsZWN0QmVoYXZpb3JhbERhdGEiOnsibmFtZSI6ImNvbGxlY3RCZWhhdmlvcmFsRGF0YSIsImRpc3BsYXlOYW1lIjoiQ29sbGVjdCBiZWhhdmlvcmFsIGRhdGEiLCJ0eXBlIjoic2VsZWN0IiwidmFsdWUiOiJ0cnVlIiwiaW5mbyI6IkJlaGF2aW9yYWwgZGF0YSBpcyB1c2VkIHRvIGRldGVjdCBIdW1hbi9Ob24gSHVtYW4gdXNlcnMuIEl0IGlzIHJlY29tbWVuZGVkIHRvIHNldCB0aGUgc2FtZSB2YWx1ZSB0aHJvdWdob3V0IHRoZSBmbG93LiIsIm9wdGlvbnMiOlt7Im5hbWUiOiJUcnVlIiwidmFsdWUiOiJ0cnVlIn0seyJuYW1lIjoiRmFsc2UiLCJ2YWx1ZSI6ImZhbHNlIn1dfSwicHJvcGVydHluYW1lIjp7Im5hbWUiOiJwcm9wZXJ0eW5hbWUiLCJkaXNwbGF5TmFtZSI6IlJpc2sgUHJvcGVydHkgTmFtZSIsInZhbHVlIjoicmlza2ZwIiwiaW5mbyI6Ik5hbWUgZm9yIHJlZmVyZW5jaW5nIHRoaXMgcmlzayBjb21wb25lbnQifX19]]]",
        "src": "auth.svg",
        "url": "skrisk",
        "children": [
          {
            "text": "skrisk"
          }
        ],
        "component": "skrisk",
        "options": {
          "environmentId": "",
          "collectBehavioralData": "true",
          "propertyname": "riskfp"
        },
        "componentProps": {
          "environmentId": {
            "name": "environmentId",
            "displayName": "Environment ID"
          },
          "collectBehavioralData": {
            "name": "collectBehavioralData",
            "displayName": "Collect behavioral data",
            "type": "select",
            "value": "true",
            "info": "Behavioral data is used to detect Human/Non Human users. It is recommended to set the same value throughout the flow.",
            "options": [
              {
                "name": "True",
                "value": "true"
              },
              {
                "name": "False",
                "value": "false"
              }
            ]
          },
          "propertyname": {
            "name": "propertyname",
            "displayName": "Risk Property Name",
            "value": "riskfp",
            "info": "Name for referencing this risk component"
          }
        },
        "tooltip": "{{component.skrisk}}"
      },
      {
        "text": ""
      },
      {
        "text": "<div  class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">  <div style="max-width: 400px; min-width: 400px; width: 100%">    <div class="card shadow mb-5">      <div class="card-body p-5 d-flex flex-column">        "
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
        "text": "        <h1 id="header" class="text-center mb-4">Password Reset</h1>        <p class="text-muted text-center">          Enter your email address and we&#39;ll send password reset instructions to you.        </p>        <p id="feedback" data-id="feedback" class="text-danger mdi mdi-alert-circle" data-skcomponent="skerror"></p>        <p class="text-danger mdi mdi-alert-circle" data-skerrorid="username" data-skcomponent="skerrormessage"></p>        <form id="usernameForm" data-id="usernameForm">          <div class="mb-4 form-floating">            <input id="username" data-id="username" class="form-control" type="text" name="username"              placeholder="Username" autocomplete="off" value="" />            <label class="form-label" for="email">Email Address</label>          </div>          <div class="d-flex flex-column">            <button id="submitBtn" data-id="submitBtn" class="btn btn-primary mb-3" type="submit"              data-skcomponent="skbutton" data-skbuttontype="form-submit" data-skform="usernameForm" data-skbuttonvalue="SUBMIT">              Submit            </button>            <button id="cancelBtn" data-id="cancelBtn" class="btn btn-link" type="submit" data-skcomponent="skbutton"              data-skbuttontype="next-event" data-skform="usernameForm" data-skbuttonvalue="CANCEL">              Cancel            </button>          </div>        </form>      </div>    </div>  </div></div>"
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




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [n9k3edxufj](./n9k3edxufj.md), [b9635u4i3w](./b9635u4i3w.md) | [c52w1izn8f](./c52w1izn8f.md) |