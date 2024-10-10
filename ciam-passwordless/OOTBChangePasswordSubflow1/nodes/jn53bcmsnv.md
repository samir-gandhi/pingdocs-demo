# Functions - Boolean Check
## Configuration
ID:  jn53bcmsnv

Type: CONNECTION 

CapabilityName: AEqualsB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Check if successShowMessage is set to true or false | 
 




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
 ```json 
boolean
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [d3ziqry02i](./d3ziqry02i.md) | [mjqbph9elz](./mjqbph9elz.md) |