# Functions - Check if Risk ID is Empty
## Configuration
ID:  hun8tkpynt

Type: CONNECTION 

CapabilityName: AIsEmpty

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | If risk ID is empty, it can be returning from subflows. | 
 




### Additional Properties
checkNullORUndefined
 ```json 
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
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [sdz87dk9h3](./sdz87dk9h3.md) | [7186msgx2b](./7186msgx2b.md) |