# Flow Connector - string 
Agreement
## Configuration
ID:  ce4oo61zup

Type: CONNECTION 

CapabilityName: startUiSubFlow






### Additional Properties
checkRequired
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


ciam_agreementEnabled
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
        "url": "ciam_agreementEnabled",
        "data": "{{global.parameters.ciam_agreementEnabled}}",
        "tooltip": "{{global.parameters.ciam_agreementEnabled}}",
        "children": [
          {
            "text": "ciam_agreementEnabled"
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


ciam_agreementId
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
        "url": "ciam_agreementId",
        "data": "{{global.parameters.ciam_agreementId}}",
        "tooltip": "{{global.parameters.ciam_agreementId}}",
        "children": [
          {
            "text": "ciam_agreementId"
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
| EVAL | [waqap3wtx](./waqap3wtx.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[3ey8zk3woh](./3ey8zk3woh.md) | 