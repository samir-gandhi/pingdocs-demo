# Functions - Check if Risk Policy ID is empty
## Configuration
ID:  wi6hu0ai62

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
| [5uyrxkfgza](./5uyrxkfgza.md) | [33jpsgsdxv](./33jpsgsdxv.md) |