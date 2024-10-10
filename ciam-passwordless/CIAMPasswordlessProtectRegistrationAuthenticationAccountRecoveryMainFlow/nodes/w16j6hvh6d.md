# PingOne Authentication - Check For Valid Session
## Configuration
ID:  w16j6hvh6d

Type: CONNECTION 

CapabilityName: checkSession

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Check if there is an existing session that&#39;s valid in current browser | 
 




### Additional Properties
authenticationMethodLastUsedIn
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
        "src": "variable.svg",
        "url": "ciam_sessionLengthInMinute",
        "data": "{{global.company.variables.ciam_sessionLengthInMinute}}",
        "tooltip": "{{global.company.variables.ciam_sessionLengthInMinute}}",
        "children": [
          {
            "text": "ciam_sessionLengthInMinute"
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


checkSessionAuthenticator
 ```json 
rememberme
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [fqkfitsm9p](./fqkfitsm9p.md) | [lbhyjujyjv](./lbhyjujyjv.md) |