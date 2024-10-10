# Functions - Check If Consent Status Is Accepted
## Configuration
ID:  1rvj1fvgpu

Type: CONNECTION 

CapabilityName: AEqualsB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




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
        "url": "status",
        "data": "{{local.8jemlov0oc.payload.output.userAgreement.status}}",
        "tooltip": "{{local.8jemlov0oc.payload.output.userAgreement.status}}",
        "children": [
          {
            "text": "status"
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
        "text": "ACCEPTED"
      }
    ]
  }
]
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [h22w6agh1](./h22w6agh1.md) | [4h6hi1onkj](./4h6hi1onkj.md) |