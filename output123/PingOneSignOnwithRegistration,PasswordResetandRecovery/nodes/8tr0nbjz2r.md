# Node - Go to Sign On Success
## Configuration
ID:  8tr0nbjz2r

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
]``` |
 




### Additional Properties
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
        "src": "pingIdentity.svg",
        "url": "email",
        "data": "{{local.icv9ot1nro.payload.output.matchedUser.email}}",
        "tooltip": "{{local.icv9ot1nro.payload.output.matchedUser.email}}",
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


nodeInstanceId
 ```json 
ofk8hitz8r
```



