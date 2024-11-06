# PingOne - string 
Find User By Username
## Configuration
ID:  4kcztxnwnw

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
        "url": "email",
        "data": "{{local.z876lbl7xg.payload.output.email}}",
        "tooltip": "{{local.z876lbl7xg.payload.output.email}}",
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
| EVAL | [bv1bbofla6](./bv1bbofla6.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[va3e8v4pwh](./va3e8v4pwh.md) | 