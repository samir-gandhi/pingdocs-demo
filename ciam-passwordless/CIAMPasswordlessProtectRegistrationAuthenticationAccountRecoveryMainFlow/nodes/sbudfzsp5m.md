# Flow Connector - Change Password
## Configuration
ID:  sbudfzsp5m

Type: CONNECTION 

CapabilityName: startUiSubFlow

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




### Additional Properties
ciam_companyLogo
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
        "src": "functions.svg",
        "url": "flowCompanyLogo",
        "data": "{{local.4rjs3llu20.payload.output.flowCompanyLogo}}",
        "tooltip": "{{local.4rjs3llu20.payload.output.flowCompanyLogo}}",
        "children": [
          {
            "text": "flowCompanyLogo"
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


showSuccessMessage
 ```json 
[
  {
    "children": [
      {
        "text": "false"
      }
    ]
  }
]
```


userID
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
        "url": "pingOneUserId",
        "data": "{{local.powvchr4kr.payload.output.pingOneUserId}}",
        "tooltip": "{{local.powvchr4kr.payload.output.pingOneUserId}}",
        "children": [
          {
            "text": "pingOneUserId"
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




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [83g36u9ohr](./83g36u9ohr.md) | [ug3m1588jl](./ug3m1588jl.md) |