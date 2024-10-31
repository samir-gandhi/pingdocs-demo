# PingOne MFA - string 
Enable MFA for user
## Configuration
ID:  up4jkblnks

Type: CONNECTION 

CapabilityName: updateUserMFAEnabled

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "pingIdentity.svg",        "url": "id",        "data": "{{local.7rwri5u6ra.payload.output.matchedUser.id}}",        "tooltip": "{{local.7rwri5u6ra.payload.output.matchedUser.id}}",        "children": [          {            "text": "id"          }        ]      },      {        "text": ""      }    ]  }] ```| 







### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [2x2le9q98](./2x2le9q98.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator |[r8nxemp506](./r8nxemp506.md) | 