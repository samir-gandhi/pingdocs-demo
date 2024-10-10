# Functions - Check if user is enabled.
## Configuration
ID:  r7ddjgug4y

Type: CONNECTION 

CapabilityName: AEqualsB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Check if the user is enabled. | 
 




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
        "url": "enabled",
        "data": "{{local.eq6oq9q1ag.payload.output.matchedUser.enabled}}",
        "tooltip": "{{local.eq6oq9q1ag.payload.output.matchedUser.enabled}}",
        "children": [
          {
            "text": "enabled"
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
        "text": "true"
      }
    ]
  }
]
```


type
 ```json 
boolean
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [71uz2oxfw9](./71uz2oxfw9.md) | [5gz6jcxdng](./5gz6jcxdng.md) |