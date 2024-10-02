# Node - Go to Sign On Success
## Configuration
ID:  scrsg9o0e2

Type: action 

CapabilityName: goToNode

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
]``` |
 




### Additional Properties
nodeInstanceId
 ```json 
ofk8hitz8r
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
        "src": "pingIdentity.svg",
        "url": "username",
        "data": "{{local.icv9ot1nro.payload.output.matchedUser.username}}",
        "tooltip": "{{local.icv9ot1nro.payload.output.matchedUser.username}}",
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



