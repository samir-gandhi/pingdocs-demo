# Flow Connector - Invoke PingOne Protect subflow
## Configuration
ID:  1vqqpdh7jj

Type: CONNECTION 

CapabilityName: startSubFlow

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Invoke PingOne Protect Sub flow for threat detection analysis using PingOne protect feature. | 
 




### Additional Properties
flowType
 ```json 
[
  {
    "children": [
      {
        "text": "REGISTRATION"
      }
    ]
  }
]
```


ipAddress
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
        "src": "auth.svg",
        "url": "ip",
        "data": "{{global.ip}}",
        "tooltip": "{{global.ip}}",
        "children": [
          {
            "text": "ip"
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


riskPolicyID
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
        "src": "variable.svg",
        "url": "ciam_protectriskPolicyId",
        "data": "{{global.variables.ciam_protectriskPolicyId}}",
        "tooltip": "{{global.variables.ciam_protectriskPolicyId}}",
        "children": [
          {
            "text": "ciam_protectriskPolicyId"
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


skriskcomponent
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
        "src": "http.svg",
        "url": "riskfp",
        "data": "{{local.z876lbl7xg.payload.output.riskfp}}",
        "tooltip": "{{local.z876lbl7xg.payload.output.riskfp}}",
        "children": [
          {
            "text": "riskfp"
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


userName
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
        "src": "http.svg",
        "url": "email",
        "data": "{{local.z876lbl7xg.payload.output.email}}",
        "tooltip": "{{local.z876lbl7xg.payload.output.email}}",
        "children": [
          {
            "text": "email"
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
| [x97hzoypsc](./x97hzoypsc.md) | [ydy90pbw5k](./ydy90pbw5k.md) |