# Flow Connector - Invoke PingOne Protect subflow
## Configuration
ID:  u9ab712lfx

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
        "text": "AUTHENTICATION"
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
        "data": "{{local.6p4frzqpp1.payload.output.riskfp}}",
        "tooltip": "{{local.6p4frzqpp1.payload.output.riskfp}}",
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
        "src": "auth.svg",
        "url": "email",
        "data": "{{global.parameters.email}}",
        "tooltip": "{{global.parameters.email}}",
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
| [qxdd8mlll5](./qxdd8mlll5.md) | [vexxoicu6a](./vexxoicu6a.md) |