# PingOne - string 
Check If User Exists
## Configuration
ID:  scja20ci5q

Type: CONNECTION 

CapabilityName: userLookup






### Additional Properties
matchAttributes
```
```


returnUserPasswordStatus
```bool 
true
```


userIdentifierForFindUser
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
        "src": "functions.svg",
        "url": "username",
        "data": "{{local.7yrdpb4c81.payload.output.username}}",
        "tooltip": "{{local.7yrdpb4c81.payload.output.username}}",
        "children": [
          {
            "text": "username"
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

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator | [avwmu6hzfh](./avwmu6hzfh.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[ld5015scb0](./ld5015scb0.md) | 