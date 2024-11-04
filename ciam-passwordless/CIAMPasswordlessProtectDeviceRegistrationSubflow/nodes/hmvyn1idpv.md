# PingOne MFA - string 
Enable MFA For User
## Configuration
ID:  hmvyn1idpv

Type: CONNECTION 

CapabilityName: updateUserMFAEnabled

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "auth.svg",        "url": "pingOneUserId",        "data": "{{global.parameters.pingOneUserId}}",        "tooltip": "{{global.parameters.pingOneUserId}}",        "children": [          {            "text": "pingOneUserId"          }        ]      },      {        "text": ""      },      {        "text": ""      },      {        "text": ""      }    ]  }] ```| 






### Additional Properties
mfaEnabled
```bool 
true
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [ug7cydwdhw](./ug7cydwdhw.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[rx5c39j4cx](./rx5c39j4cx.md) | 