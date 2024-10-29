# PingOne - string 
Lookup User
## Configuration
ID:  2ernrgqxzb

Type: CONNECTION 

CapabilityName: userLookup

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
Searches for the user in PingOne&#39;s cloud directory | 





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
        "data": "{{local.rmx6s73ihv.payload.output.email}}",
        "tooltip": "{{local.rmx6s73ihv.payload.output.email}}",
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
| EVAL | [1nt8111fdv](./1nt8111fdv.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[71chk8uoyb](./71chk8uoyb.md) | 