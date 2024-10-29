# Functions - string 
Is MFA Enabled?
## Configuration
ID:  j8lmuiytzs

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
        "url": "mfaEnabled",
        "data": "{{local.ms19ql02hi.payload.output.mfaEnabled}}",
        "tooltip": "{{local.ms19ql02hi.payload.output.mfaEnabled}}",
        "children": [
          {
            "text": "mfaEnabled"
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
        "text": "true"
      }
    ]
  }
]
```


type
```string 
boolean
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [fd7o3icva4](./fd7o3icva4.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[bf9jlbogz1](./bf9jlbogz1.md) | 