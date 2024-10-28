# Functions - string 
Risk Score from PingOne Protect
## Configuration
ID:  o4xxassgqz

Type: CONNECTION 

CapabilityName: AEqualsMultipleB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
Branching based on risk score from PingOne Protect | 





### Additional Properties
caseSensitive
```bool 
false
```


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
| EVAL | [lonpqbsfiu](./lonpqbsfiu.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[4tfnhsx2bw](./4tfnhsx2bw.md) | 