# PingOne - Check User Consent Status
## Configuration
ID:  8jemlov0oc

Type: CONNECTION 

CapabilityName: checkUserAgreement

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




### Additional Properties
agreementId
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


identifier
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
        "url": "pingOneUserId",
        "data": "{{global.parameters.pingOneUserId}}",
        "tooltip": "{{global.parameters.pingOneUserId}}",
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
| [prjjhhmndv](./prjjhhmndv.md) | [h22w6agh1](./h22w6agh1.md) |