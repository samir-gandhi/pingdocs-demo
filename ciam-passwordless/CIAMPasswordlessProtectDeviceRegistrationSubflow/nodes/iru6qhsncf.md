# PingOne MFA - Activate FIDO2 Device
## Configuration
ID:  iru6qhsncf

Type: CONNECTION 

CapabilityName: activateDevice

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```[  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "auth.svg",        "url": "pingOneUserId",        "data": "{{global.parameters.pingOneUserId}}",        "tooltip": "{{global.parameters.pingOneUserId}}",        "children": [          {            "text": "pingOneUserId"          }        ]      },      {        "text": ""      }    ]  }] ```| 

 




### Additional Properties
attestation
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
        "text": ""
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "http.svg",
        "url": "attestationValue",
        "data": "{{local.6jkz2hx974.payload.output.attestationValue}}",
        "tooltip": "{{local.6jkz2hx974.payload.output.attestationValue}}",
        "children": [
          {
            "text": "attestationValue"
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


deviceId
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
        "url": "id",
        "data": "{{local.5y2z6x314y.payload.output.device.id}}",
        "tooltip": "{{local.5y2z6x314y.payload.output.device.id}}",
        "children": [
          {
            "text": "id"
          }
        ]
      },
      {
        "text": ""
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


origin
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
        "url": "origin",
        "data": "{{local.vc8o1wnpis.payload.output.origin}}",
        "tooltip": "{{local.vc8o1wnpis.payload.output.origin}}",
        "children": [
          {
            "text": "origin"
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
| [wpljz4km80](./wpljz4km80.md) | [h7w9k7knl9](./h7w9k7knl9.md) |