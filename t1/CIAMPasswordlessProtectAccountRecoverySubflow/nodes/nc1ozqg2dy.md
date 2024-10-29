# PingOne - string 
Disable User
## Configuration
ID:  nc1ozqg2dy

Type: CONNECTION 

CapabilityName: enableUser






### Additional Properties
identifier
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
        "url": "email",
        "data": "{{local.g3ie4cp1z5.payload.output.matchedUser.email}}",
        "tooltip": "{{local.g3ie4cp1z5.payload.output.matchedUser.email}}",
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


matchAttribute
```string 
email
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [jozexysssa](./jozexysssa.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[ymg2y1p8tf](./ymg2y1p8tf.md) | 