# PingOne - Find user in PingOne
## Configuration
ID:  eq6oq9q1ag

Type: CONNECTION 

CapabilityName: userLookup

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Find user by Username or email as entered in login page | 
 




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
        "url": "useremail",
        "data": "{{local.nyw41b5mjr.payload.output.useremail}}",
        "tooltip": "{{local.nyw41b5mjr.payload.output.useremail}}",
        "children": [
          {
            "text": "useremail"
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
| [iui85ujva3](./iui85ujva3.md) | [71uz2oxfw9](./71uz2oxfw9.md) |