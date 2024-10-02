# PingOne - Update password
## Configuration
ID:  0c41v9ejkb

Type: action 

CapabilityName: resetPassword

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Updates the user&#39;s password to the new one submitted if current password was validated | }
 




### Additional Properties
currentPassword
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
        "url": "currentPassword",
        "data": "{{local.h9q1e6iiu0.payload.output.currentPassword}}",
        "tooltip": "{{local.h9q1e6iiu0.payload.output.currentPassword}}",
        "children": [
          {
            "text": "currentPassword"
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


identifier
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
        "url": "userId",
        "data": "{{local.ercttap70x.payload.output.userId}}",
        "tooltip": "{{local.ercttap70x.payload.output.userId}}",
        "children": [
          {
            "text": "userId"
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


newPassword
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
        "url": "newPassword",
        "data": "{{local.h9q1e6iiu0.payload.output.newPassword}}",
        "tooltip": "{{local.h9q1e6iiu0.payload.output.newPassword}}",
        "children": [
          {
            "text": "newPassword"
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



