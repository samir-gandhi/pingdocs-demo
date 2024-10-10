# PingOne - Find user and error out if user not found
## Configuration
ID:  8a3rp16jhq

Type: CONNECTION 

CapabilityName: userLookup

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




### Additional Properties
matchAttributes
 ```json 

```


useCustomSCIMFilter
 ```json 
false
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
        "data": "{{local.dv7x4k323t.payload.output.email}}",
        "tooltip": "{{local.dv7x4k323t.payload.output.email}}",
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
| [ncdawmfdmo](./ncdawmfdmo.md) | [ybma422b3i](./ybma422b3i.md) |