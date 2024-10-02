# PingOne - Validate verification code
## Configuration
ID:  jw8ez5s8p8

Type: action 

CapabilityName: verifyEmail

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Sends the verification code to PingOne to validate | }
 




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
        "data": "{{local.agjdg5vxr2.payload.output.user.id}}",
        "tooltip": "{{local.agjdg5vxr2.payload.output.user.id}}",
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


verificationCode
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
        "url": "verificationCode",
        "data": "{{local.qojn9nsdxh.payload.output.verificationCode}}",
        "tooltip": "{{local.qojn9nsdxh.payload.output.verificationCode}}",
        "children": [
          {
            "text": "verificationCode"
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



