# PingOne - string 
Find user details
## Configuration
ID:  yj3z2ix7ge

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
        "src": "http.svg",
        "url": "username",
        "data": "{{local.klrsk927mu.payload.output.username}}",
        "tooltip": "{{local.klrsk927mu.payload.output.username}}",
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
| EVAL | [lonpqbsfiu](./lonpqbsfiu.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[82g5jqcpg1](./82g5jqcpg1.md) | 