# PingOne - Check If User Exists
## Configuration
ID:  scja20ci5q

Type: CONNECTION 

CapabilityName: userLookup

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




### Additional Properties
matchAttributes
 ```json 

```


returnUserPasswordStatus
 ```json 
true
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
        "src": "functions.svg",
        "url": "username",
        "data": "{{local.7yrdpb4c81.payload.output.username}}",
        "tooltip": "{{local.7yrdpb4c81.payload.output.username}}",
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
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [avwmu6hzfh](./avwmu6hzfh.md) | [ld5015scb0](./ld5015scb0.md) |