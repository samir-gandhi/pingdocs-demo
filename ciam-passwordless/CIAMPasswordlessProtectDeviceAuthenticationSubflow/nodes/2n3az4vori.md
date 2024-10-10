# Functions - User Has Active Devices
## Configuration
ID:  2n3az4vori

Type: CONNECTION 

CapabilityName: AGreaterThanB

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
        "src": "functions.svg",
        "url": "count",
        "data": "{{local.10uwd1ccc4.payload.output.count}}",
        "tooltip": "{{local.10uwd1ccc4.payload.output.count}}",
        "children": [
          {
            "text": "count"
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
        "text": "0"
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
| [bf9jlbogz1](./bf9jlbogz1.md) | [0sua91hqk7](./0sua91hqk7.md) |