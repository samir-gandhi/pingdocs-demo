# PingOne MFA - string 
Read all MFA devices
## Configuration
ID:  bcrh9zpo2j

Type: CONNECTION 

CapabilityName: readAllDevices

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "pingIdentity.svg",        "url": "id",        "data": "{{local.flt9ewj1a9.payload.output.matchedUser.id}}",        "tooltip": "{{local.flt9ewj1a9.payload.output.matchedUser.id}}",        "children": [          {            "text": "id"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Node Description | string 
Read all MFA devices | 





### Additional Properties
setFilterFlag
```bool 
true
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [0cmw42tqse](./0cmw42tqse.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[1gv745vu9f](./1gv745vu9f.md) | 