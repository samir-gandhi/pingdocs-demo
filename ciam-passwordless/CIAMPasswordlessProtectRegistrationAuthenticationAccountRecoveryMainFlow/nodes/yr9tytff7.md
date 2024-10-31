# PingOne Authentication - string 
Redirect With Error Response
## Configuration
ID:  yr9tytff7

Type: CONNECTION 

CapabilityName: returnErrorResponseRedirect

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Background Color | html 
#ffc8c1ff | 






### Additional Properties
customErrorFlag
```bool 
true
```


errorDescription
```json 
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
        "src": "teleport.svg",
        "url": "errorMessage",
        "data": "{{local.cl9ugbu07r.payload.output.errorMessage}}",
        "tooltip": "{{local.cl9ugbu07r.payload.output.errorMessage}}",
        "children": [
          {
            "text": "errorMessage"
          }
        ]
      },
      {
        "text": ""
      }
    ]
  }
]
```


errorMessage
```string 
invalid_request
```




