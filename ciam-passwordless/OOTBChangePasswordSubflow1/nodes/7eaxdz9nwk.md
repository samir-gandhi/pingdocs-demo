# PingOne - Update password
## Configuration
ID:  7eaxdz9nwk

Type: CONNECTION 

CapabilityName: resetPassword

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




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
        "data": "{{local.5vfn623mx7.payload.output.currentPassword}}",
        "tooltip": "{{local.5vfn623mx7.payload.output.currentPassword}}",
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
        "src": "auth.svg",
        "url": "userID",
        "data": "{{global.parameters.userID}}",
        "tooltip": "{{global.parameters.userID}}",
        "children": [
          {
            "text": "userID"
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
        "data": "{{local.5vfn623mx7.payload.output.newPassword}}",
        "tooltip": "{{local.5vfn623mx7.payload.output.newPassword}}",
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




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [6oeo7c9bch](./6oeo7c9bch.md) | [ateb0l10nl](./ateb0l10nl.md) |