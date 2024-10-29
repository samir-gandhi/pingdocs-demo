# PingOne MFA - string 
Continue MFA With Only Device
## Configuration
ID:  b01n00fwkm

Type: CONNECTION 

CapabilityName: deviceSelectDeviceAuthentication






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
        "text": ""
      },
      {
        "type": "link",
        "src": "pingIdentity.svg",
        "url": "id",
        "data": "{{local.10oaokas61.payload.output.rawResponse.id}}",
        "tooltip": "{{local.10oaokas61.payload.output.rawResponse.id}}",
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
        "text": "{{local.9m5a2f4emp.payload.output.rawResponse._embedded.devices[0].id}}"
      }
    ]
  }
]
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [ayodtok1lb](./ayodtok1lb.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[47qta86y95](./47qta86y95.md) | 