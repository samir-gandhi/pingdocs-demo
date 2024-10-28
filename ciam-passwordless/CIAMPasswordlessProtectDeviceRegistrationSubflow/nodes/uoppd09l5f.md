# PingOne MFA - string 
Activate OTP Device
## Configuration
ID:  uoppd09l5f

Type: CONNECTION 

CapabilityName: activateDevice

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "auth.svg",        "url": "pingOneUserId",        "data": "{{global.parameters.pingOneUserId}}",        "tooltip": "{{global.parameters.pingOneUserId}}",        "children": [          {            "text": "pingOneUserId"          }        ]      },      {        "text": ""      }    ]  }] ```| 






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
        "text": ""
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "variable.svg",
        "url": "ciam_deviceId",
        "data": "{{global.variables.ciam_deviceId}}",
        "tooltip": "{{global.variables.ciam_deviceId}}",
        "children": [
          {
            "text": "ciam_deviceId"
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
        "text": ""
      },
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
        "text": ""
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "teleport.svg",
        "url": "otp",
        "data": "{{local.7qi7idcwvv.payload.output.otp}}",
        "tooltip": "{{local.7qi7idcwvv.payload.output.otp}}",
        "children": [
          {
            "text": "otp"
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
| EVAL | [ih33zryjpu](./ih33zryjpu.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[ug7cydwdhw](./ug7cydwdhw.md) | 