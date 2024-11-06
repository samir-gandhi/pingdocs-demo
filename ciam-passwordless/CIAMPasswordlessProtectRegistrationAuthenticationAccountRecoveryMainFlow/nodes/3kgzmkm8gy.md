# Functions - string 
Check if  user is enabled.
## Configuration
ID:  3kgzmkm8gy

Type: CONNECTION 

CapabilityName: AEqualsB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
Check if  user is enabled. | 





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
```string 
boolean
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [3e86t7q5xg](./3e86t7q5xg.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[vconl69bto](./vconl69bto.md) | 