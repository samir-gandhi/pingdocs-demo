# Functions - Check if Risk ID is Empty
## Configuration
ID:  0cdm5xwnl3

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
| [2ixdpv74ih](./2ixdpv74ih.md) | [oep2ke136](./oep2ke136.md) |