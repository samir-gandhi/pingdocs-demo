# Functions - string 
Check MFA devices size
## Configuration
ID:  nf4hv96sui

Type: CONNECTION 

CapabilityName: AEqualsB






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
        "src": "pingIdentity.svg",
        "url": "size",
        "data": "{{local.9m5a2f4emp.payload.output.rawResponse.size}}",
        "tooltip": "{{local.9m5a2f4emp.payload.output.rawResponse.size}}",
        "children": [
          {
            "text": "size"
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
```string 
number
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [n69ynlsgag](./n69ynlsgag.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator |[mtaqacdw1m](./mtaqacdw1m.md) | 