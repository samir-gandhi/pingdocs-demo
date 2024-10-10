# Functions - Check if Risk Policy ID is empty
## Configuration
ID:  dxowhkk5n5

Type: CONNECTION 

CapabilityName: AIsEmpty

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Check if Risk Policy ID is empty | 
 




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
| [iloobtovwh](./iloobtovwh.md) | [kgxiu8h9i5](./kgxiu8h9i5.md) |