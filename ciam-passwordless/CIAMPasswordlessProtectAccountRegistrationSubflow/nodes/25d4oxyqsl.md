# Http - string 
Error
## Configuration
ID:  25d4oxyqsl

Type: CONNECTION 

CapabilityName: createErrorResponse

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Background Color | html 
#ffc8c1ff | 






### Additional Properties
claimsNameValuePairs
```
```


message
```json 
[
  {
    "children": [
      {
        "text": "Error"
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "url:ctt831xici",
        "url": "errorCode",
        "data": "{{local.prajl7in65.payload.output.errorCode}}",
        "tooltip": "{{local.prajl7in65.payload.output.errorCode}}",
        "children": [
          {
            "text": "{{local.prajl7in65.payload.output.errorCode}}"
          }
        ]
      },
      {
        "text": " - "
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "teleport.svg",
        "url": "errorMessage",
        "data": "{{local.prajl7in65.payload.output.errorMessage}}",
        "tooltip": "{{local.prajl7in65.payload.output.errorMessage}}",
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
        "text": ""
      }
    ]
  }
]
```




