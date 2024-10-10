# Functions - Risk Score from PingOne Protect
## Configuration
ID:  o4xxassgqz

Type: CONNECTION 

CapabilityName: AEqualsMultipleB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Branching based on risk score from PingOne Protect | 
 




### Additional Properties
caseSensitive
 ```json 
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
 ```json 

```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [8u4731kx7c](./8u4731kx7c.md), [lonpqbsfiu](./lonpqbsfiu.md) | [f4he7cr9jf](./f4he7cr9jf.md), [tr6ask2nn2](./tr6ask2nn2.md), [4tfnhsx2bw](./4tfnhsx2bw.md) |