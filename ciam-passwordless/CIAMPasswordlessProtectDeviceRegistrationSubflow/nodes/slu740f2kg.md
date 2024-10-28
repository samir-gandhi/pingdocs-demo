# PingOne MFA - string 
Delete Previous Device
## Configuration
ID:  slu740f2kg

Type: CONNECTION 

CapabilityName: deleteDevice

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "auth.svg",        "url": "pingOneUserId",        "data": "{{global.parameters.pingOneUserId}}",        "tooltip": "{{global.parameters.pingOneUserId}}",        "children": [          {            "text": "pingOneUserId"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Node Description | string 
Delete the non activated device to create a new one instead | 





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

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [h00gom93pv](./h00gom93pv.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[wdmeq58d57](./wdmeq58d57.md) | 