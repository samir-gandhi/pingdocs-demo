# Functions - string 
Check If MFA Is enabled?
## Configuration
ID:  rsj0knmukp

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
        "data": "{{local.7rwri5u6ra.payload.output.matchedUser.mfaEnabled}}",
        "tooltip": "{{local.7rwri5u6ra.payload.output.matchedUser.mfaEnabled}}",
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
| EVAL | [rxrwt223m5](./rxrwt223m5.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator |[3jsczqq7hm](./3jsczqq7hm.md) | 