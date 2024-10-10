# Flow Connector - CIAM - Device Authentication
## Configuration
ID:  eht5fkf5yz

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
        "text": ""
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "teleport.svg",
        "url": "flowAllowedDeviceTypes",
        "data": "{{local.el9cmscetd.payload.output.flowAllowedDeviceTypes}}",
        "tooltip": "{{local.el9cmscetd.payload.output.flowAllowedDeviceTypes}}",
        "children": [
          {
            "text": "flowAllowedDeviceTypes"
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


ciam_magicLinkEnabled
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
        "url": "flowMagicLinkEnabled",
        "data": "{{local.el9cmscetd.payload.output.flowMagicLinkEnabled}}",
        "tooltip": "{{local.el9cmscetd.payload.output.flowMagicLinkEnabled}}",
        "children": [
          {
            "text": "flowMagicLinkEnabled"
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
        "src": "http.svg",
        "url": "email",
        "data": "{{local.rmx6s73ihv.payload.output.email}}",
        "tooltip": "{{local.rmx6s73ihv.payload.output.email}}",
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
        "data": "{{global.company.variables.ciam_magicLinkEnabled}}",
        "tooltip": "{{global.company.variables.ciam_magicLinkEnabled}}",
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


magicLinkRegistered
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
        "src": "pingIdentity.svg",
        "url": "id",
        "data": "{{local.2ernrgqxzb.payload.output.matchedUser.id}}",
        "tooltip": "{{local.2ernrgqxzb.payload.output.matchedUser.id}}",
        "children": [
          {
            "text": "id"
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


username
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
        "data": "{{local.pjpixj6e2f.payload.output.username}}",
        "tooltip": "{{local.pjpixj6e2f.payload.output.username}}",
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
| [71chk8uoyb](./71chk8uoyb.md) | [hp2eob8gy8](./hp2eob8gy8.md) |