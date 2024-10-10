# PingOne - Find user details
## Configuration
ID:  yj3z2ix7ge

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
        "url": "username",
        "data": "{{local.klrsk927mu.payload.output.username}}",
        "tooltip": "{{local.klrsk927mu.payload.output.username}}",
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
| [lonpqbsfiu](./lonpqbsfiu.md) | [82g5jqcpg1](./82g5jqcpg1.md) |