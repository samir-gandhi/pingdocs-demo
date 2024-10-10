# PingOne MFA - Enable MFA For User
## Configuration
ID:  hmvyn1idpv

Type: CONNECTION 

CapabilityName: updateUserMFAEnabled

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```[  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "auth.svg",        "url": "pingOneUserId",        "data": "{{global.parameters.pingOneUserId}}",        "tooltip": "{{global.parameters.pingOneUserId}}",        "children": [          {            "text": "pingOneUserId"          }        ]      },      {        "text": ""      },      {        "text": ""      },      {        "text": ""      }    ]  }] ```| 

 




### Additional Properties
mfaEnabled
 ```json 
true
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [ug7cydwdhw](./ug7cydwdhw.md) | [rx5c39j4cx](./rx5c39j4cx.md) |