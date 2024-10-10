# PingOne MFA - Read all MFA devices
## Configuration
ID:  bcrh9zpo2j

Type: CONNECTION 

CapabilityName: readAllDevices

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```[  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "pingIdentity.svg",        "url": "id",        "data": "{{local.flt9ewj1a9.payload.output.matchedUser.id}}",        "tooltip": "{{local.flt9ewj1a9.payload.output.matchedUser.id}}",        "children": [          {            "text": "id"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Node Description | Read all MFA devices | 
 




### Additional Properties
setFilterFlag
 ```json 
true
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [0cmw42tqse](./0cmw42tqse.md) | [1gv745vu9f](./1gv745vu9f.md) |