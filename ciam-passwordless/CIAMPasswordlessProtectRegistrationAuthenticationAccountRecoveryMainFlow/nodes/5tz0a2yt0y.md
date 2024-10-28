# Functions - string 
Check if MFA Size is 0
## Configuration
ID:  5tz0a2yt0y

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
        "data": "{{local.bcrh9zpo2j.payload.output.rawResponse.size}}",
        "tooltip": "{{local.bcrh9zpo2j.payload.output.rawResponse.size}}",
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
| EVAL | [1gv745vu9f](./1gv745vu9f.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator |[opojvoak73](./opojvoak73.md) | 