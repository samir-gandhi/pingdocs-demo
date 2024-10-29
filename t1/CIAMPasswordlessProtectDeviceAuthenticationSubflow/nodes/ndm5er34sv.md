# Functions - string 
Risk Score from PingOne Protect
## Configuration
ID:  ndm5er34sv

Type: CONNECTION 

CapabilityName: AEqualsMultipleB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
Branching based on risk score from PingOne Protect | 





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
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [nl0cxyid0x](./nl0cxyid0x.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[sk3dza5671](./sk3dza5671.md) | 