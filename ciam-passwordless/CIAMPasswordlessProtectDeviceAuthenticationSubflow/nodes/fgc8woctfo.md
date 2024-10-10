# PingOne MFA - Validate Passcode
## Configuration
ID:  fgc8woctfo

Type: CONNECTION 

CapabilityName: validateOtpDeviceAuthentication

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




### Additional Properties
deviceAuthenticationId
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
        "text": ""
      },
      {
        "type": "link",
        "src": "teleport.svg",
        "url": "deviceAuthId",
        "data": "{{local.zxfluj3oxa.payload.output.deviceAuthId}}",
        "tooltip": "{{local.zxfluj3oxa.payload.output.deviceAuthId}}",
        "children": [
          {
            "text": "deviceAuthId"
          }
        ]
      },
      {
        "text": ""
      },
      {
        "text": ""
      }
    ]
  }
]
```


otp
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
        "url": "passcode",
        "data": "{{local.r6lnkuy0yh.payload.output.passcode}}",
        "tooltip": "{{local.r6lnkuy0yh.payload.output.passcode}}",
        "children": [
          {
            "text": "passcode"
          }
        ]
      },
      {
        "text": ""
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
| [mt9kvt7hnn](./mt9kvt7hnn.md) | [7vrrd3uuhm](./7vrrd3uuhm.md) |