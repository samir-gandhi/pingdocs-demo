# PingOne - Lookup User
## Configuration
ID:  2ernrgqxzb

Type: CONNECTION 

CapabilityName: userLookup

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Searches for the user in PingOne&#39;s cloud directory | 
 




### Additional Properties
matchAttributes
 ```json 

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
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [1nt8111fdv](./1nt8111fdv.md) | [71chk8uoyb](./71chk8uoyb.md) |