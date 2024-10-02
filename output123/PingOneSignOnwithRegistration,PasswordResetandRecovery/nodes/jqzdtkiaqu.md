# PingOne - Set new password
## Configuration
ID:  jqzdtkiaqu

Type: action 

CapabilityName: recoverPassword

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID | ```json[
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
        "data": "{{local.n0w3iu8ao3.payload.output.matchedUser.id}}",
        "tooltip": "{{local.n0w3iu8ao3.payload.output.matchedUser.id}}",
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
]``` |
| Node Description | Sets a new password if the user exists and the submitted recovery code is valid | }
 




### Additional Properties
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
        "src": "pingIdentity.svg",
        "url": "id",
        "data": "{{local.n0w3iu8ao3.payload.output.matchedUser.id}}",
        "tooltip": "{{local.n0w3iu8ao3.payload.output.matchedUser.id}}",
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
        "data": "{{local.fkekf3oi8e.payload.output.newPassword}}",
        "tooltip": "{{local.fkekf3oi8e.payload.output.newPassword}}",
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


recoverPassword_localizedErrors
 ```json 

```


recoveryCode
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
        "url": "recoveryCode",
        "data": "{{local.fkekf3oi8e.payload.output.recoveryCode}}",
        "tooltip": "{{local.fkekf3oi8e.payload.output.recoveryCode}}",
        "children": [
          {
            "text": "recoveryCode"
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



