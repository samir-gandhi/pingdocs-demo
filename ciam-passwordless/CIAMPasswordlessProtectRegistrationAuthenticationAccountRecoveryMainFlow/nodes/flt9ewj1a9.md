# PingOne - string 
Find user via userID
## Configuration
ID:  flt9ewj1a9

Type: CONNECTION 

CapabilityName: userLookup






### Additional Properties
matchAttributes
```
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
        "src": "teleport.svg",
        "url": "pingOneUserId",
        "data": "{{local.h2wapsopzt.payload.output.pingOneUserId}}",
        "tooltip": "{{local.h2wapsopzt.payload.output.pingOneUserId}}",
        "children": [
          {
            "text": "pingOneUserId"
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
| EVAL | [y2yl45morr](./y2yl45morr.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[k3qn24f8pv](./k3qn24f8pv.md) | 