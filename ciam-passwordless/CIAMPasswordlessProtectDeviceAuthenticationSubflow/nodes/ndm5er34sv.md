# Functions - Risk Score from PingOne Protect
## Configuration
ID:  ndm5er34sv

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
| [x8ainlbr6x](./x8ainlbr6x.md), [nl0cxyid0x](./nl0cxyid0x.md) | [4n12f0orqv](./4n12f0orqv.md), [n69ynlsgag](./n69ynlsgag.md), [sk3dza5671](./sk3dza5671.md) |