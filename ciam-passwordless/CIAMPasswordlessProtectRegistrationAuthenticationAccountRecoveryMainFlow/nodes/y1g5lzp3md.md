# Functions - string 
Did Subflow Return Success
## Configuration
ID:  y1g5lzp3md

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
        "src": "flow-connector.svg",
        "url": "ciam_subflowResult",
        "data": "{{local.sbudfzsp5m.payload.output.ciam_subflowResult}}",
        "tooltip": "{{local.sbudfzsp5m.payload.output.ciam_subflowResult}}",
        "children": [
          {
            "text": "ciam_subflowResult"
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
        "text": "Success"
      }
    ]
  }
]
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator | [ug3m1588jl](./ug3m1588jl.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[8b7afymuxh](./8b7afymuxh.md) | 