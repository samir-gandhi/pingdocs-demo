# Functions - Does user currently have password?
## Configuration
ID:  40jmo5fihf

Type: CONNECTION 

CapabilityName: AEqualsB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




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
        "url": "passwordStatus",
        "data": "{{local.scja20ci5q.payload.output.passwordStatus}}",
        "tooltip": "{{local.scja20ci5q.payload.output.passwordStatus}}",
        "children": [
          {
            "text": "passwordStatus"
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


type
 ```json 
string
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [ld5015scb0](./ld5015scb0.md) | [0lyofgg9w1](./0lyofgg9w1.md) |