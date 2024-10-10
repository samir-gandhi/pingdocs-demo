# Flow Connector - Check Agreement
## Configuration
ID:  frkr1a0u82

Type: CONNECTION 

CapabilityName: startUiSubFlow

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




### Additional Properties
checkRequired
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
        "src": "teleport.svg",
        "url": "flowAgreementEnabled",
        "data": "{{local.1r9qfce4ko.payload.output.flowAgreementEnabled}}",
        "tooltip": "{{local.1r9qfce4ko.payload.output.flowAgreementEnabled}}",
        "children": [
          {
            "text": "flowAgreementEnabled"
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
        "src": "teleport.svg",
        "url": "flowAgreementId",
        "data": "{{local.1r9qfce4ko.payload.output.flowAgreementId}}",
        "tooltip": "{{local.1r9qfce4ko.payload.output.flowAgreementId}}",
        "children": [
          {
            "text": "flowAgreementId"
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
        "data": "{{local.1r9qfce4ko.payload.output.pingOneUserId}}",
        "tooltip": "{{local.1r9qfce4ko.payload.output.pingOneUserId}}",
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
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [76t9hosyif](./76t9hosyif.md) | [r01x04oq1y](./r01x04oq1y.md) |