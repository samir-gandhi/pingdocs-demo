# Functions - Check account status
## Configuration
ID:  4ncwrpsqgn

Type: CONNECTION 

CapabilityName: AEqualsB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Check if account status is Active | 
 




### Additional Properties
leftValueA
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
        "url": "status",
        "data": "{{local.eq6oq9q1ag.payload.output.matchedUser.account.status}}",
        "tooltip": "{{local.eq6oq9q1ag.payload.output.matchedUser.account.status}}",
        "children": [
          {
            "text": "status"
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


rightValueB
 ```json 
[
  {
    "children": [
      {
        "text": "OK"
      }
    ]
  }
]
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [fm7p6z4lgt](./fm7p6z4lgt.md) | [ph08u6bgi1](./ph08u6bgi1.md) |