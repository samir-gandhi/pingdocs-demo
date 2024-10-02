# PingOne - User Lookup
## Configuration
ID:  cqm26fxq1v

Type: action 

CapabilityName: userLookup

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Attempts to find the user in PingOne by the submitted username | }
 




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
        "url": "username",
        "data": "{{local.cq77vwelou.payload.output.username}}",
        "tooltip": "{{local.cq77vwelou.payload.output.username}}",
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


userLookup_localizedErrors
 ```json 

```



