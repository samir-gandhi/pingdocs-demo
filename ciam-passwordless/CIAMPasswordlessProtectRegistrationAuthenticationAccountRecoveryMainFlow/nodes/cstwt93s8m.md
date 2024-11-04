# Functions - string 
Check Password Status
## Configuration
ID:  cstwt93s8m

Type: CONNECTION 

CapabilityName: AEqualsMultipleB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
Branches based on the password status returned by PingOne | 





### Additional Properties
leftValueA
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
        "url": "status",
        "data": "{{local.us1sbucx0m.payload.output.rawResponse.status}}",
        "tooltip": "{{local.us1sbucx0m.payload.output.rawResponse.status}}",
        "children": [
          {
            "text": "status"
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


rightValueMultiple
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [c9kmm14iq0](./c9kmm14iq0.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[nbcsfwxqvp](./nbcsfwxqvp.md) | 