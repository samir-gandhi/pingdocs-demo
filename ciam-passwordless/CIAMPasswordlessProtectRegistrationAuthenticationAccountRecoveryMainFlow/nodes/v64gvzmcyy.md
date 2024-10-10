# Functions - Check if MFA is enabled to this user.
## Configuration
ID:  v64gvzmcyy

Type: CONNECTION 

CapabilityName: AEqualsB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Check if MFA is enabled to this user. | 
 




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
        "url": "mfaEnabled",
        "data": "{{local.eq6oq9q1ag.payload.output.matchedUser.mfaEnabled}}",
        "tooltip": "{{local.eq6oq9q1ag.payload.output.matchedUser.mfaEnabled}}",
        "children": [
          {
            "text": "mfaEnabled"
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
| [dfcr1art1l](./dfcr1art1l.md) | [fm7p6z4lgt](./fm7p6z4lgt.md) |