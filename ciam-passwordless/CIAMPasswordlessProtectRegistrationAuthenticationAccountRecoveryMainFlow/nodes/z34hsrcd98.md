# Flow Connector - string 
CIAM - Account Recovery 
## Configuration
ID:  z34hsrcd98

Type: CONNECTION 

CapabilityName: startUiSubFlow






### Additional Properties
ciam_companyLogo
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
        "src": "functions.svg",
        "url": "flowCompanyLogo",
        "data": "{{local.4rjs3llu20.payload.output.flowCompanyLogo}}",
        "tooltip": "{{local.4rjs3llu20.payload.output.flowCompanyLogo}}",
        "children": [
          {
            "text": "flowCompanyLogo"
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


passwordRecovery
```json 
[
  {
    "children": [
      {
        "text": "false"
      }
    ]
  }
]
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [wcask7tfhv](./wcask7tfhv.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[21l7s55n2w](./21l7s55n2w.md) | 