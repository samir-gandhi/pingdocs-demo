# Flow Connector - string 
Device Registration
## Configuration
ID:  hbtxkrrfyo

Type: CONNECTION 

CapabilityName: startUiSubFlow






### Additional Properties
allowCancel
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


allowedDeviceTypes
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
        "url": "allowedDeviceTypes",
        "data": "{{global.parameters.allowedDeviceTypes}}",
        "tooltip": "{{global.parameters.allowedDeviceTypes}}",
        "children": [
          {
            "text": "allowedDeviceTypes"
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


ciam_autoEnrollEmail
```json 
[
  {
    "children": [
      {
        "text": "true"
      }
    ]
  }
]
```


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
        "src": "auth.svg",
        "url": "ciam_companyLogo",
        "data": "{{global.parameters.ciam_companyLogo}}",
        "tooltip": "{{global.parameters.ciam_companyLogo}}",
        "children": [
          {
            "text": "ciam_companyLogo"
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


email
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
        "url": "email",
        "data": "{{local.i2k2g4dd4k.payload.output.email}}",
        "tooltip": "{{local.i2k2g4dd4k.payload.output.email}}",
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


passwordlessRequired
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
        "url": "ciam_passwordlessRequired",
        "data": "{{global.parameters.ciam_passwordlessRequired}}",
        "tooltip": "{{global.parameters.ciam_passwordlessRequired}}",
        "children": [
          {
            "text": "ciam_passwordlessRequired"
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


pingOneUserId
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
        "data": "{{local.i2k2g4dd4k.payload.output.pingOneUserId}}",
        "tooltip": "{{local.i2k2g4dd4k.payload.output.pingOneUserId}}",
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

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [r6sues2bxt](./r6sues2bxt.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator |[8euk2r8qqp](./8euk2r8qqp.md) | 