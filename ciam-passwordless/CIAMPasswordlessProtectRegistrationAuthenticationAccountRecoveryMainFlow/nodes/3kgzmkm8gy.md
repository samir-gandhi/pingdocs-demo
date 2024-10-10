# Functions - Check if  user is enabled.
## Configuration
ID:  3kgzmkm8gy

Type: CONNECTION 

CapabilityName: AEqualsB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Check if  user is enabled. | 
 




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
        "data": "{{local.8a3rp16jhq.payload.output.matchedUser.enabled}}",
        "tooltip": "{{local.8a3rp16jhq.payload.output.matchedUser.enabled}}",
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
| [3e86t7q5xg](./3e86t7q5xg.md) | [vconl69bto](./vconl69bto.md) |