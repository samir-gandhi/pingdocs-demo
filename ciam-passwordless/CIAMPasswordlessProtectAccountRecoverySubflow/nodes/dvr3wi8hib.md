# Functions - string 
Split By User&#39;s Selection
## Configuration
ID:  dvr3wi8hib

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
        "data": "{{local.klrsk927mu.payload.output.buttonValue}}",
        "tooltip": "{{local.klrsk927mu.payload.output.buttonValue}}",
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
| EVAL | [c52w1izn8f](./c52w1izn8f.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[v28wjjz61p](./v28wjjz61p.md) | 