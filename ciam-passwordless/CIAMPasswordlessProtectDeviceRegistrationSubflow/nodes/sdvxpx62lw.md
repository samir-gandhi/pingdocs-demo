# Functions - Check If User Can Auto Enroll?
## Configuration
ID:  sdvxpx62lw

Type: CONNECTION 

CapabilityName: AEqualsB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | User&#39;s email will be auto enrolled, assuming the email is already verified in the calling flow | 
 




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
        "src": "auth.svg",
        "url": "ciam_autoEnrollEmail",
        "data": "{{global.parameters.ciam_autoEnrollEmail}}",
        "tooltip": "{{global.parameters.ciam_autoEnrollEmail}}",
        "children": [
          {
            "text": "ciam_autoEnrollEmail"
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
 ```json 
boolean
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [4smjdpxvyk](./4smjdpxvyk.md) | [zdzabypfcv](./zdzabypfcv.md) |