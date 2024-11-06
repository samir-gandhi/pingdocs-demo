# Functions - string 
Split By User&#39;s Selection
## Configuration
ID:  rtv1hwltfy

Type: CONNECTION 

CapabilityName: AEqualsMultipleB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
Branch based on the button selected on the forgot password form | 





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
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [n9tgrbpiz4](./n9tgrbpiz4.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[t6hyz30ejn](./t6hyz30ejn.md) | 