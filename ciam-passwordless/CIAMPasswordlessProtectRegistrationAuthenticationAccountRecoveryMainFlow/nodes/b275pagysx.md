# Functions - string 
Is Account Locked?
## Configuration
ID:  b275pagysx

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
        "url": "code",
        "data": "{{local.us1sbucx0m.payload.error.code}}",
        "tooltip": "{{local.us1sbucx0m.payload.error.code}}",
        "children": [
          {
            "text": "code"
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
        "text": "passwordLockedOut"
      }
    ]
  }
]
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [c9kmm14iq0](./c9kmm14iq0.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[scxeegwacj](./scxeegwacj.md) | 