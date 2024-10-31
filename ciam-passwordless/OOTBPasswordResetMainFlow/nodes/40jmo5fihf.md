# Functions - string 
Does user currently have password?
## Configuration
ID:  40jmo5fihf

Type: CONNECTION 

CapabilityName: AEqualsB






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
```string 
string
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [ld5015scb0](./ld5015scb0.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[0lyofgg9w1](./0lyofgg9w1.md) | 