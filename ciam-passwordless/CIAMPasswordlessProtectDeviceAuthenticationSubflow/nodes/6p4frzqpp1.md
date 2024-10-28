# Http - string 
Get Origin
## Configuration
ID:  6p4frzqpp1

Type: CONNECTION 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
Get Origin and initialise skrisk | 

## Custom CSS
```css
json 
.hidden-button{
    display: none;
}
```

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
        "text": "<form id="location" method="post">    <input type="hidden" name="origin" id="origin">    <input type="hidden" name="rpid" id="rpid">    <button type="hidden" data-skcomponent="skbutton" data-skbuttontype="form-submit" class="hidden-button"  data-skbuttonvalue="submit" data-skform="location" id="autoSubmit">Next</button></form>"
      }
    ]
  }
]
```

## Custom Script
```js 
setTimeout(function() {
    const origin = window.location.origin;
    document.getElementById("origin").value = origin;
    // const index = origin.indexOf("pingone.");
        const index = origin.indexOf(":");
        const index2 = index &#43; 3;
    document.getElementById("rpid").value = origin.substr(index2);
    document.getElementById(&#39;autoSubmit&#39;).click();
}, 1000);
```


### Additional Properties
formFieldsList
```
```




