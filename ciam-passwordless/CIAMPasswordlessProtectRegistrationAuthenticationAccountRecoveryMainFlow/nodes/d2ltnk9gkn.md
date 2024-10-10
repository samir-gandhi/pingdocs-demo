# PingOne Notifications - Notify user on disabling the account for threat detection.
## Configuration
ID:  d2ltnk9gkn

Type: CONNECTION 

CapabilityName: sendEmail

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```[  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "pingIdentity.svg",        "url": "id",        "data": "{{local.flt9ewj1a9.payload.output.matchedUser.id}}",        "tooltip": "{{local.flt9ewj1a9.payload.output.matchedUser.id}}",        "children": [          {            "text": "id"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Node Description | Notify user on disabling the account for threat detection. | 
 




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
        "data": "{{local.flt9ewj1a9.payload.output.matchedUser.email}}",
        "tooltip": "{{local.flt9ewj1a9.payload.output.matchedUser.email}}",
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
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [qvyge7omps](./qvyge7omps.md) | [1v3t743uow](./1v3t743uow.md) |