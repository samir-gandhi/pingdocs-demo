# Functions - Split By User&#39;s Selection
## Configuration
ID:  rtv1hwltfy

Type: CONNECTION 

CapabilityName: AEqualsMultipleB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Branch based on the button selected on the forgot password form | 
 




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
        "src": "http.svg",
        "url": "buttonValue",
        "data": "{{local.h4u1as8yg4.payload.output.buttonValue}}",
        "tooltip": "{{local.h4u1as8yg4.payload.output.buttonValue}}",
        "children": [
          {
            "text": "buttonValue"
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
        "text": "submit"
      }
    ]
  }
]
```


rightValueMultiple
 ```json 

```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [n9tgrbpiz4](./n9tgrbpiz4.md) | [bl9wn96q7z](./bl9wn96q7z.md), [fecpsdg3u3](./fecpsdg3u3.md), [t6hyz30ejn](./t6hyz30ejn.md) |