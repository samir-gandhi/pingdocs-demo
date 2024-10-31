# Functions - string 
Empty Check
## Configuration
ID:  h330sqhk7o

Type: CONNECTION 

CapabilityName: AIsEmpty

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
Check if showSuccessMessage is empty | 





### Additional Properties
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
        "src": "auth.svg",
        "url": "showSuccessMessage",
        "data": "{{global.parameters.showSuccessMessage}}",
        "tooltip": "{{global.parameters.showSuccessMessage}}",
        "children": [
          {
            "text": "showSuccessMessage"
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


type
```string 
boolean
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator | [ateb0l10nl](./ateb0l10nl.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[d3ziqry02i](./d3ziqry02i.md) | 