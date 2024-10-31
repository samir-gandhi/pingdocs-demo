# PingOne MFA - string 
Delete Device
## Configuration
ID:  powjrjqmwn

Type: CONNECTION 

CapabilityName: deleteDevice

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "teleport.svg",        "url": "userId",        "data": "{{local.ebzcromrpm.payload.output.userId}}",        "tooltip": "{{local.ebzcromrpm.payload.output.userId}}",        "children": [          {            "text": "userId"          }        ]      },      {        "text": ""      }    ]  }] ```| 






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





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [dpv60nrlu4](./dpv60nrlu4.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[921411zeq1](./921411zeq1.md) | 