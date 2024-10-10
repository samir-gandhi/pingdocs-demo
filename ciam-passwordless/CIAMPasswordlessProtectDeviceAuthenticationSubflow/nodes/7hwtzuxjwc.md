# PingOne - Disable user
## Configuration
ID:  7hwtzuxjwc

Type: CONNECTION 

CapabilityName: enableUser

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




### Additional Properties
identifier
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


matchAttribute
 ```json 
email
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [iz5nper189](./iz5nper189.md) | [99q38lg97t](./99q38lg97t.md) |