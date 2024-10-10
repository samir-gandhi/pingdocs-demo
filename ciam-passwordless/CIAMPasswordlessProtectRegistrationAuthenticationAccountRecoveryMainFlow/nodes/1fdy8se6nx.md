# PingOne Protect - Update risk evaluation with FAILURE
## Configuration
ID:  1fdy8se6nx

Type: CONNECTION 

CapabilityName: updateRiskEvaluation

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




### Additional Properties
completionStatus
 ```json 
[
  {
    "children": [
      {
        "text": "FAILED"
      }
    ]
  }
]
```


riskId
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
        "url": "ciam_protectRiskID",
        "data": "{{global.variables.ciam_protectRiskID}}",
        "tooltip": "{{global.variables.ciam_protectRiskID}}",
        "children": [
          {
            "text": "ciam_protectRiskID"
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




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [oep2ke136](./oep2ke136.md) |  |