# PingOne MFA - string 
Set Device As Default
## Configuration
ID:  v9xx0rido4

Type: CONNECTION 

CapabilityName: setDeviceOrder

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "teleport.svg",        "url": "userId",        "data": "{{local.ebzcromrpm.payload.output.userId}}",        "tooltip": "{{local.ebzcromrpm.payload.output.userId}}",        "children": [          {            "text": "userId"          }        ]      },      {        "text": ""      }    ]  }] ```| 






### Additional Properties
defaultDeviceId
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


setDeviceOrder
```string 
SET_DEFAULT_DEVICE
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [fvt3dt1sk1](./fvt3dt1sk1.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[c6dxhfi5rb](./c6dxhfi5rb.md) | 