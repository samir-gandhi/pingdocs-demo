# Functions - Risk Score from PingOne Protect
## Configuration
ID:  uekzlj66vx

Type: CONNECTION 

CapabilityName: AEqualsMultipleB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Branching based on risk score from PingOne Protect | 
 




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
        "src": "variable.svg",
        "url": "ciam_protectRiskLevel",
        "data": "{{global.variables.ciam_protectRiskLevel}}",
        "tooltip": "{{global.variables.ciam_protectRiskLevel}}",
        "children": [
          {
            "text": "ciam_protectRiskLevel"
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
| [0eroz3r95x](./0eroz3r95x.md), [gaj3ygo1j4](./gaj3ygo1j4.md) | [oc2cqsl41l](./oc2cqsl41l.md), [0cmw42tqse](./0cmw42tqse.md), [80hktgiwnm](./80hktgiwnm.md) |