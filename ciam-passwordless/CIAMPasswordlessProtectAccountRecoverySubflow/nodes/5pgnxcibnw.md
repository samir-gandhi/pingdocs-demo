# PingOne Notifications - PingOne Notifications
## Configuration
ID:  5pgnxcibnw

Type: CONNECTION 

CapabilityName: sendEmail

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```[  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "pingIdentity.svg",        "url": "id",        "data": "{{local.yj3z2ix7ge.payload.output.matchedUser.id}}",        "tooltip": "{{local.yj3z2ix7ge.payload.output.matchedUser.id}}",        "children": [          {            "text": "id"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Node Description | Configure email notification | 
 




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
        "data": "{{local.yj3z2ix7ge.payload.output.matchedUser.email}}",
        "tooltip": "{{local.yj3z2ix7ge.payload.output.matchedUser.email}}",
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
| [82g5jqcpg1](./82g5jqcpg1.md) | [8u4731kx7c](./8u4731kx7c.md) |