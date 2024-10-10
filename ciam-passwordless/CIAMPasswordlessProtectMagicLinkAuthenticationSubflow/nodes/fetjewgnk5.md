# PingOne Notifications - Send Magic Link Email
## Configuration
ID:  fetjewgnk5

Type: CONNECTION 

CapabilityName: sendEmail

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```[  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "pingIdentity.svg",        "url": "id",        "data": "{{local.n6qy3v9bsy.payload.output.matchedUser.id}}",        "tooltip": "{{local.n6qy3v9bsy.payload.output.matchedUser.id}}",        "children": [          {            "text": "id"          }        ]      },      {        "text": ""      }    ]  }] ```| 

 




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
        "src": "auth.svg",
        "url": "email",
        "data": "{{global.parameters.email}}",
        "tooltip": "{{global.parameters.email}}",
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


templateVariables
 ```json 

```


templateVariant
 ```json 
Magic Link
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [65s242z206](./65s242z206.md) | [ali9zum89s](./ali9zum89s.md) |