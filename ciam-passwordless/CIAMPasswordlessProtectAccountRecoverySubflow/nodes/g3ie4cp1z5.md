# PingOne - string 
Find user details
## Configuration
ID:  g3ie4cp1z5

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
| EVAL | [8fh7taswpw](./8fh7taswpw.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[0gubix0onw](./0gubix0onw.md) | 