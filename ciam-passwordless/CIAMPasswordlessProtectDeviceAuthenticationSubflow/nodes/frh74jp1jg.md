# Functions - Only One Usable Device
## Configuration
ID:  frh74jp1jg

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
        "text": "1"
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
| [v0t14r4lv2](./v0t14r4lv2.md) | [ydyrhm9fkz](./ydyrhm9fkz.md) |