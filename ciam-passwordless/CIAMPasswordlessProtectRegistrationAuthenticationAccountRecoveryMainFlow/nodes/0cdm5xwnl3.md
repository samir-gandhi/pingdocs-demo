# Functions - string 
Check if Risk ID is Empty
## Configuration
ID:  0cdm5xwnl3

Type: CONNECTION 

CapabilityName: AIsEmpty

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
If risk ID is empty, it can be returning from subflows. | 





### Additional Properties
checkNullORUndefined
```bool 
true
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

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [2ixdpv74ih](./2ixdpv74ih.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator |[oep2ke136](./oep2ke136.md) | 