# Flow Connector - Invoke PingOne Protect subflow
## Configuration
ID:  m71wjatj9v

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
        "data": "{{local.klrsk927mu.payload.output.riskfp}}",
        "tooltip": "{{local.klrsk927mu.payload.output.riskfp}}",
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
        "url": "username",
        "data": "{{local.klrsk927mu.payload.output.username}}",
        "tooltip": "{{local.klrsk927mu.payload.output.username}}",
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
| [zpg6zu1p21](./zpg6zu1p21.md) | [pz7469or4k](./pz7469or4k.md) |