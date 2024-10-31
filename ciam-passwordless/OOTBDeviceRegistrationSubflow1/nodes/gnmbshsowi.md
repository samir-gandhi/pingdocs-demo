# Functions - string 
Is Error Invalid Phone Number/Email Address?
## Configuration
ID:  gnmbshsowi

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
        "data": "{{local.pjzv5pikab.payload.error.code}}",
        "tooltip": "{{local.pjzv5pikab.payload.error.code}}",
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
        "text": "invalidValue"
      }
    ]
  }
]
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [thtxgh5tye](./thtxgh5tye.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[2my7xaouma](./2my7xaouma.md) | 