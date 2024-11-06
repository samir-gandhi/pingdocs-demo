# Functions - string 
Risk Score from PingOne Protect
## Configuration
ID:  uekzlj66vx

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
| EVAL | [gaj3ygo1j4](./gaj3ygo1j4.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[80hktgiwnm](./80hktgiwnm.md) | 