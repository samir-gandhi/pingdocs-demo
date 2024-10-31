# Functions - string 
Check if Risk Policy ID is empty
## Configuration
ID:  wi6hu0ai62

Type: CONNECTION 

CapabilityName: AIsEmpty

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
Check if Risk Policy ID is empty | 





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
| EVAL | [5uyrxkfgza](./5uyrxkfgza.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[33jpsgsdxv](./33jpsgsdxv.md) | 