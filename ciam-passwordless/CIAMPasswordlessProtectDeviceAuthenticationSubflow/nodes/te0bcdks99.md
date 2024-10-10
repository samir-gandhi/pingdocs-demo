# Flow Connector - Magic Link Authentication
## Configuration
ID:  te0bcdks99

Type: CONNECTION 

CapabilityName: startUiSubFlow

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




### Additional Properties
allowedDeviceTypes
 ```json 
[
  {
    "children": [
      {
        "text": "SMS, EMAIL, PLATFORM"
      }
    ]
  }
]
```


anyMfaDevices
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


canChangeDevice
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


hideSkipButton
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


magicLinkEnabled
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
        "url": "ciam_magicLinkEnabled",
        "data": "{{global.variables.ciam_magicLinkEnabled}}",
        "tooltip": "{{global.variables.ciam_magicLinkEnabled}}",
        "children": [
          {
            "text": "ciam_magicLinkEnabled"
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


p1UserId
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
        "url": "pingUserId",
        "data": "{{global.parameters.pingUserId}}",
        "tooltip": "{{global.parameters.pingUserId}}",
        "children": [
          {
            "text": "pingUserId"
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


pingUserId
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
        "data": "{{local.52wlmnlym3.payload.output.pingOneUserId}}",
        "tooltip": "{{local.52wlmnlym3.payload.output.pingOneUserId}}",
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


returnResponse
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




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [vul5k2q2dw](./vul5k2q2dw.md) | [qsu3efxcsp](./qsu3efxcsp.md) |