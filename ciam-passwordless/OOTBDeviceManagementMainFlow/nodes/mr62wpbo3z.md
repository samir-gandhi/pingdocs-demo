# PingOne MFA - Update Device Name
## Configuration
ID:  mr62wpbo3z

Type: CONNECTION 

CapabilityName: updateDeviceNickname

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```[  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "teleport.svg",        "url": "userId",        "data": "{{local.ebzcromrpm.payload.output.userId}}",        "tooltip": "{{local.ebzcromrpm.payload.output.userId}}",        "children": [          {            "text": "userId"          }        ]      },      {        "text": ""      }    ]  }] ```| 

 




### Additional Properties
deviceId
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
        "url": "deviceId",
        "data": "{{local.ebzcromrpm.payload.output.deviceId}}",
        "tooltip": "{{local.ebzcromrpm.payload.output.deviceId}}",
        "children": [
          {
            "text": "deviceId"
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


nickname
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
        "url": "nickname",
        "data": "{{local.j4l954l5hz.payload.output.nickname}}",
        "tooltip": "{{local.j4l954l5hz.payload.output.nickname}}",
        "children": [
          {
            "text": "nickname"
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
| [0mbvscfh8v](./0mbvscfh8v.md) | [cb42qgfnjd](./cb42qgfnjd.md) |