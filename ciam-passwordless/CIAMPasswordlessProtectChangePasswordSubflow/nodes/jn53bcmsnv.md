# Functions - string 
Boolean Check
## Configuration
ID:  jn53bcmsnv

Type: CONNECTION 

CapabilityName: AEqualsB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
Check if successShowMessage is set to true or false | 





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


rightValueB
```json 
[
  {
    "children": [
      {
        "text": "true"
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
| EVAL | [d3ziqry02i](./d3ziqry02i.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator |[mjqbph9elz](./mjqbph9elz.md) | 