# PingOne - Validate Password
## Configuration
ID:  dnu7jt3sjz

Type: action 

CapabilityName: checkPassword

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
        "data": "{{local.icv9ot1nro.payload.output.matchedUser.id}}",
        "tooltip": "{{local.icv9ot1nro.payload.output.matchedUser.id}}",
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
| Node Description | Validates that the user submitted the correct password for the account associated with the username | }
 




### Additional Properties
checkPassword_localizedErrors
 ```json 

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
        "src": "pingIdentity.svg",
        "url": "id",
        "data": "{{local.cqm26fxq1v.payload.output.matchedUser.id}}",
        "tooltip": "{{local.cqm26fxq1v.payload.output.matchedUser.id}}",
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


matchAttribute
 ```json 
id
```


password
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
        "url": "password",
        "data": "{{local.cq77vwelou.payload.output.password}}",
        "tooltip": "{{local.cq77vwelou.payload.output.password}}",
        "children": [
          {
            "text": "password"
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



