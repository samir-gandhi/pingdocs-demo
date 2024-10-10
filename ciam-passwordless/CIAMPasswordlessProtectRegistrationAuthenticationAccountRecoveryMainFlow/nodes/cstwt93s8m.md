# Functions - Check Password Status
## Configuration
ID:  cstwt93s8m

Type: CONNECTION 

CapabilityName: AEqualsMultipleB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Branches based on the password status returned by PingOne | 
 




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
 ```json 

```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [c9kmm14iq0](./c9kmm14iq0.md) | [rqsigpn591](./rqsigpn591.md), [imnmdfh12z](./imnmdfh12z.md), [nbcsfwxqvp](./nbcsfwxqvp.md) |