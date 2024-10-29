# PingOne Notifications - string 
PingOne Notifications
## Configuration
ID:  ahjplbui3q

Type: CONNECTION 

CapabilityName: sendEmail

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "pingIdentity.svg",        "url": "id",        "data": "{{local.3y03qc0kxe.payload.output.matchedUser.id}}",        "tooltip": "{{local.3y03qc0kxe.payload.output.matchedUser.id}}",        "children": [          {            "text": "id"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Node Description | string 
Configure email notification | 





### Additional Properties
customTemplateVariant
```json 
{}
```


email
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
        "src": "pingIdentity.svg",
        "url": "email",
        "data": "{{local.3y03qc0kxe.payload.output.matchedUser.email}}",
        "tooltip": "{{local.3y03qc0kxe.payload.output.matchedUser.email}}",
        "children": [
          {
            "text": "email"
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
| EVAL | [nl0cxyid0x](./nl0cxyid0x.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[x8ainlbr6x](./x8ainlbr6x.md) | 