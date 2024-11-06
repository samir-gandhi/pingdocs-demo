# Flow Connector - string 
Verify Email
## Configuration
ID:  q2xj7vprwc

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
        "src": "auth.svg",
        "url": "ciam_companyLogo",
        "data": "{{global.parameters.ciam_companyLogo}}",
        "tooltip": "{{global.parameters.ciam_companyLogo}}",
        "children": [
          {
            "text": "ciam_companyLogo"
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


pingOneUserId
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
        "src": "teleport.svg",
        "url": "pingOneUserId",
        "data": "{{local.i2k2g4dd4k.payload.output.pingOneUserId}}",
        "tooltip": "{{local.i2k2g4dd4k.payload.output.pingOneUserId}}",
        "children": [
          {
            "text": "pingOneUserId"
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





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [3ey8zk3woh](./3ey8zk3woh.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[yauguijv8y](./yauguijv8y.md) | 