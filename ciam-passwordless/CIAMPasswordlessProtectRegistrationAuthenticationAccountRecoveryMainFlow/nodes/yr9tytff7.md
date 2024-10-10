# PingOne Authentication - Redirect With Error Response
## Configuration
ID:  yr9tytff7

Type: CONNECTION 

CapabilityName: returnErrorResponseRedirect

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Background Color | #ffc8c1ff | 

 




### Additional Properties
customErrorFlag
 ```json 
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
 ```json 
invalid_request
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [yjz1weh9xh](./yjz1weh9xh.md) |  |