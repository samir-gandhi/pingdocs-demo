# PingOne - Find User By Username
## Configuration
ID:  4kcztxnwnw

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
        "src": "http.svg",
        "url": "email",
        "data": "{{local.z876lbl7xg.payload.output.email}}",
        "tooltip": "{{local.z876lbl7xg.payload.output.email}}",
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
| [bv1bbofla6](./bv1bbofla6.md) | [va3e8v4pwh](./va3e8v4pwh.md) |