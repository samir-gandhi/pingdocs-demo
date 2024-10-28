# Functions - string 
Check if Risk ID is Empty
## Configuration
ID:  hun8tkpynt

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
| EVAL | [sdz87dk9h3](./sdz87dk9h3.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator |[7186msgx2b](./7186msgx2b.md) | 