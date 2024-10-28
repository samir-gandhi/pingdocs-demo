# Functions - string 
Does User Have Existing Password
## Configuration
ID:  ux2xzdhk0a

Type: CONNECTION 

CapabilityName: ANotEqualsB






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
        "url": "passwordStatus",
        "data": "{{local.0jvt7xvej2.payload.output.passwordStatus}}",
        "tooltip": "{{local.0jvt7xvej2.payload.output.passwordStatus}}",
        "children": [
          {
            "text": "passwordStatus"
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
        "text": "NO_PASSWORD"
      }
    ]
  }
]
```


type
```string 
string
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [mcc4xn7khm](./mcc4xn7khm.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[eph6l2tfnr](./eph6l2tfnr.md) | 