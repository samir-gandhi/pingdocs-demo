# Functions - Does User Have Existing Password
## Configuration
ID:  ux2xzdhk0a

Type: CONNECTION 

CapabilityName: ANotEqualsB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




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
        "url": "passwordStatus",
        "data": "{{local.0jvt7xvej2.payload.output.passwordStatus}}",
        "tooltip": "{{local.0jvt7xvej2.payload.output.passwordStatus}}",
        "children": [
          {
            "text": "passwordStatus"
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


rightValueB
 ```json 
[
  {
    "children": [
      {
        "text": "NO_PASSWORD"
      }
    ]
  }
]
```


type
 ```json 
string
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [mcc4xn7khm](./mcc4xn7khm.md) | [eph6l2tfnr](./eph6l2tfnr.md) |