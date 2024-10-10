# PingOne - Find user via userID
## Configuration
ID:  flt9ewj1a9

Type: CONNECTION 

CapabilityName: userLookup

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




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
        "src": "teleport.svg",
        "url": "pingOneUserId",
        "data": "{{local.h2wapsopzt.payload.output.pingOneUserId}}",
        "tooltip": "{{local.h2wapsopzt.payload.output.pingOneUserId}}",
        "children": [
          {
            "text": "pingOneUserId"
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
| [y2yl45morr](./y2yl45morr.md) | [k3qn24f8pv](./k3qn24f8pv.md) |