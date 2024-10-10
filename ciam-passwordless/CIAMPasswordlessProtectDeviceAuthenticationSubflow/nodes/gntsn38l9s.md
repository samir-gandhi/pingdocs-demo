# Flow Connector - CIAM - Magic Link Authentication
## Configuration
ID:  gntsn38l9s

Type: CONNECTION 

CapabilityName: startUiSubFlow

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




### Additional Properties
anyMfaDevices
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
        "url": "success",
        "data": "{{local.2n3az4vori.payload.success}}",
        "tooltip": "{{local.2n3az4vori.payload.success}}",
        "children": [
          {
            "text": "success"
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


canChangeDevice
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


mfaEnabled
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
        "url": "success",
        "data": "{{local.2n3az4vori.payload.success}}",
        "tooltip": "{{local.2n3az4vori.payload.success}}",
        "children": [
          {
            "text": "success"
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
| [7vz1yqkdqo](./7vz1yqkdqo.md) | [51zazld6jz](./51zazld6jz.md) |