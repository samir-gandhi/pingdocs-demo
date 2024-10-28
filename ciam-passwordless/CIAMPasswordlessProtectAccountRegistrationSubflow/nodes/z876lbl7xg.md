# Http - string 
Email Form
## Configuration
ID:  z876lbl7xg

Type: CONNECTION 

CapabilityName: customHTMLTemplate



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
        "text": "<div  class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">  <div style="max-width: 400px; min-width: 400px; width: 100%"">    <div class="card shadow mb-5">      <div class="card-body p-5 d-flex flex-column">        "
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
        "text": "        <h1 id="header" class="text-center mb-4">Create Your Profile</h1>        <p id="feedback" data-id="feedback" class="text-danger mdi mdi-alert-circle" data-skcomponent="skerror"></p>        <p class="text-danger mdi mdi-alert-circle" data-skerrorid="email" data-skcomponent="skerrormessage"></p>        <form id="registrationForm" data-id="registrationForm">          <div class="mb-4 form-floating">            <input id="email" data-id="email" class="form-control" type="text" name="email" placeholder="Email Address" autocomplete="off" />            <label id="emailLabel" data-id="emailLabel" class="form-label" for="email">Email Address</label>          </div>          <div class="d-flex flex-column">            <button id="submitBtn" data-id="submitBtn" class="btn btn-primary mb-3" type="submit" data-skcomponent="skbutton"               data-skbuttontype="form-submit" data-skform="registrationForm" data-skbuttonvalue="REGISTER">                Create Account            </button>            <div class="d-flex flex-column">              <button id="cancelBtn" data-id="cancelBtn" class="btn btn-link" type="submit" data-skcomponent="skbutton"                data-skbuttontype="next-event" data-skform="registrationForm" data-skbuttonvalue="SIGNON">                Already have an account? Sign on              </button>            </div>          </div>        </form>      </div>    </div>  </div></div>"
      }
    ]
  }
]
```



### Additional Properties
formFieldsList
```
```


validationRules
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [9ajkfnvew2](./9ajkfnvew2.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[tew5x0pd7f](./tew5x0pd7f.md) | 