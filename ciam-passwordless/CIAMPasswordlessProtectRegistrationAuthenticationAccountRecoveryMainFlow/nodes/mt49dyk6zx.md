# Flow Connector - Invoke PingOne Protect subflow
## Configuration
ID:  mt49dyk6zx

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
        "src": "teleport.svg",
        "url": "SKRiskId",
        "data": "{{local.h2wapsopzt.payload.output.SKRiskId}}",
        "tooltip": "{{local.h2wapsopzt.payload.output.SKRiskId}}",
        "children": [
          {
            "text": "SKRiskId"
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
        "src": "pingIdentity.svg",
        "url": "username",
        "data": "{{local.flt9ewj1a9.payload.output.matchedUser.username}}",
        "tooltip": "{{local.flt9ewj1a9.payload.output.matchedUser.username}}",
        "children": [
          {
            "text": "username"
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
| [k3qn24f8pv](./k3qn24f8pv.md) | [w5t7jozp5a](./w5t7jozp5a.md) |