# PingOne - string 
User Lookup
## Configuration
ID:  t09lk8opxa

Type: CONNECTION 

CapabilityName: userLookup

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
Attempts to find the user in PingOne by the submitted username | 





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
        "text": ""
      },
      {
        "type": "link",
        "src": "http.svg",
        "url": "username",
        "data": "{{local.howu8n9hsc.payload.output.username}}",
        "tooltip": "{{local.howu8n9hsc.payload.output.username}}",
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
        "url": "email",
        "data": "{{local.rstodi2zw1.payload.output.email}}",
        "tooltip": "{{local.rstodi2zw1.payload.output.email}}",
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


userLookup_localizedErrors
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [bilu0ighwr](./bilu0ighwr.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[y7f4468q9f](./y7f4468q9f.md) | 