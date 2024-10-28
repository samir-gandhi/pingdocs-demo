# PingOne MFA - string 
Enable MFA for user
## Configuration
ID:  v92cr3znpj

Type: CONNECTION 

CapabilityName: updateUserMFAEnabled

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "auth.svg",        "url": "pingOneUserId",        "data": "{{global.parameters.pingOneUserId}}",        "tooltip": "{{global.parameters.pingOneUserId}}",        "children": [          {            "text": "pingOneUserId"          }        ]      },      {        "text": ""      }    ]  }] ```| 






### Additional Properties
mfaEnabled
```bool 
true
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [h7w9k7knl9](./h7w9k7knl9.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[qj9x404zi1](./qj9x404zi1.md) | 