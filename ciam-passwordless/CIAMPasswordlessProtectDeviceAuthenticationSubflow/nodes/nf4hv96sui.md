# Functions - Check MFA devices size
## Configuration
ID:  nf4hv96sui

Type: CONNECTION 

CapabilityName: AEqualsB

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
        "url": "size",
        "data": "{{local.9m5a2f4emp.payload.output.rawResponse.size}}",
        "tooltip": "{{local.9m5a2f4emp.payload.output.rawResponse.size}}",
        "children": [
          {
            "text": "size"
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
        "text": "0"
      }
    ]
  }
]
```


type
 ```json 
number
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [n69ynlsgag](./n69ynlsgag.md) | [mtaqacdw1m](./mtaqacdw1m.md) |