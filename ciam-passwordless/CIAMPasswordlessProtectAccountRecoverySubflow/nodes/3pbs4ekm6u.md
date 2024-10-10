# Functions - Is Validation Limit Reached?
## Configuration
ID:  3pbs4ekm6u

Type: CONNECTION 

CapabilityName: ALessThanB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




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
        "src": "variable.svg",
        "url": "ciam_recoveryValidationAttempts",
        "data": "{{global.variables.ciam_recoveryValidationAttempts}}",
        "tooltip": "{{global.variables.ciam_recoveryValidationAttempts}}",
        "children": [
          {
            "text": "ciam_recoveryValidationAttempts"
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
        "text": ""
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "variable.svg",
        "url": "ciam_recoveryLimit",
        "data": "{{global.company.variables.ciam_recoveryLimit}}",
        "tooltip": "{{global.company.variables.ciam_recoveryLimit}}",
        "children": [
          {
            "text": "ciam_recoveryLimit"
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
 ```json 
number
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [xkvo347q5m](./xkvo347q5m.md) | [1brhauigps](./1brhauigps.md) |