# PingOne - Find user details
## Configuration
ID:  3y03qc0kxe

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
        "src": "auth.svg",
        "url": "pingOneUserId",
        "data": "{{global.parameters.pingOneUserId}}",
        "tooltip": "{{global.parameters.pingOneUserId}}",
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
| [pt24r4nafa](./pt24r4nafa.md) | [qxdd8mlll5](./qxdd8mlll5.md) |