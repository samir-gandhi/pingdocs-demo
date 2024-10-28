# Functions - string 
Check If User Needs To Enter Email
## Configuration
ID:  7mu81oaiqx

Type: CONNECTION 

CapabilityName: AIsEmpty






### Additional Properties
checkNullORUndefined
```bool 
true
```


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
        "src": "auth.svg",
        "url": "email",
        "data": "{{global.parameters.email}}",
        "tooltip": "{{global.parameters.email}}",
        "children": [
          {
            "text": "email"
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
| EVAL | [k90u9roz6q](./k90u9roz6q.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[4smjdpxvyk](./4smjdpxvyk.md) | 