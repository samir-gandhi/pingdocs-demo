# PingOne - string 
Find user in PingOne
## Configuration
ID:  eq6oq9q1ag

Type: CONNECTION 

CapabilityName: userLookup

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
Find user by Username or email as entered in login page | 





### Additional Properties
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

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [iui85ujva3](./iui85ujva3.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator |[71uz2oxfw9](./71uz2oxfw9.md) | 