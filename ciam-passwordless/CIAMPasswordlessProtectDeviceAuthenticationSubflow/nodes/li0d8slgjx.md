# PingOne Notifications - string 
Send email for new device
## Configuration
ID:  li0d8slgjx

Type: CONNECTION 

CapabilityName: sendEmail

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "pingIdentity.svg",        "url": "id",        "data": "{{local.3y03qc0kxe.payload.output.matchedUser.id}}",        "tooltip": "{{local.3y03qc0kxe.payload.output.matchedUser.id}}",        "children": [          {            "text": "id"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Node Description | string 
Configure email notification to send an email for new device added. | 





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
| EVAL | [qw4n733f3t](./qw4n733f3t.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[e3httj56zd](./e3httj56zd.md) | 