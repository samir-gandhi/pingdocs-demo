# Functions - Is Passwordless Not Required?
## Configuration
ID:  i8me302hqi

Type: CONNECTION 

CapabilityName: AEqualsB

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
        "src": "auth.svg",
        "url": "ciam_passwordlessRequired",
        "data": "{{global.parameters.ciam_passwordlessRequired}}",
        "tooltip": "{{global.parameters.ciam_passwordlessRequired}}",
        "children": [
          {
            "text": "ciam_passwordlessRequired"
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
        "text": "false"
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
| [x3sr98yxnv](./x3sr98yxnv.md) | [a2zg9lz4ta](./a2zg9lz4ta.md) |