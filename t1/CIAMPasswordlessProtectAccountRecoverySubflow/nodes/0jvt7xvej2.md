# PingOne - string 
Lookup User
## Configuration
ID:  0jvt7xvej2

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
| EVAL | [k0gh9sf1l8](./k0gh9sf1l8.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[mcc4xn7khm](./mcc4xn7khm.md) | 