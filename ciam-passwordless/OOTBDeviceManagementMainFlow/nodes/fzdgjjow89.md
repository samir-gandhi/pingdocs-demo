# Http - Error Screen
## Configuration
ID:  fzdgjjow89

Type: CONNECTION 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 


## Custom HTML
```html
[
  {
    "children": [
      {
        "text": "<div\tclass="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">\t<div class="mh-100" style="max-width: 400px; width: 100%;">\t\t<div class="card shadow mb-5">\t\t\t<div class="card-body p-5 d-flex flex-column">\t\t\t\t<img                    class="align-self-center mb-5"                    src=""
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "variable.svg",
        "url": "ciam_logoUrl",
        "data": "{{global.company.variables.ciam_logoUrl}}",
        "tooltip": "{{global.company.variables.ciam_logoUrl}}",
        "children": [
          {
            "text": "{{global.company.variables.ciam_logoUrl}}"
          }
        ]
      },
      {
        "text": ""
      },
      {
        "text": ""                    alt=""
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "variable.svg",
        "url": "ciam_companyName",
        "data": "{{global.company.variables.ciam_companyName}}",
        "tooltip": "{{global.company.variables.ciam_companyName}}",
        "children": [
          {
            "text": "{{global.company.variables.ciam_companyName}}"
          }
        ]
      },
      {
        "text": ""
      },
      {
        "text": ""                    style=""
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "variable.svg",
        "url": "ciam_logoStyle",
        "data": "{{global.company.variables.ciam_logoStyle}}",
        "tooltip": "{{global.company.variables.ciam_logoStyle}}",
        "children": [
          {
            "text": "{{global.company.variables.ciam_logoStyle}}"
          }
        ]
      },
      {
        "text": ""
      },
      {
        "text": ""                />\t\t\t\t<h1 class="text-center mb-4">Error</h1>\t\t\t\t<p class="text-muted text-center">\t\t\t\t\t"
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "teleport.svg",
        "url": "errorMessage",
        "data": "{{local.at5tmglpow.payload.output.errorMessage}}",
        "tooltip": "{{local.at5tmglpow.payload.output.errorMessage}}",
        "children": [
          {
            "text": "errorMessage"
          }
        ]
      },
      {
        "text": ""
      },
      {
        "text": "\t\t\t\t</p>\t\t\t\t<button data-id="button" type="submit" class="btn btn-primary mb-3" data-skcomponent="skbutton"\t\t\t\t\tdata-skbuttontype="form-submit" data-skform="form" id="btnContinue"\t\t\t\t\tdata-skbuttonvalue="CONTINUE">\t\t\t\t\tContinue\t\t\t\t</button>\t\t\t</div>\t\t</div>\t</div></div>"
      }
    ]
  }
]
```


### Additional Properties
formFieldsList
 ```json 

```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [6rcgg8opng](./6rcgg8opng.md) | [miwpvke4ky](./miwpvke4ky.md) |