# PingOne - Disable User
## Configuration
ID:  nc1ozqg2dy

Type: CONNECTION 

CapabilityName: enableUser

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




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
        "type": "link",
        "src": "pingIdentity.svg",
        "url": "email",
        "data": "{{local.g3ie4cp1z5.payload.output.matchedUser.email}}",
        "tooltip": "{{local.g3ie4cp1z5.payload.output.matchedUser.email}}",
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


matchAttribute
 ```json 
email
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [jozexysssa](./jozexysssa.md) | [ymg2y1p8tf](./ymg2y1p8tf.md) |