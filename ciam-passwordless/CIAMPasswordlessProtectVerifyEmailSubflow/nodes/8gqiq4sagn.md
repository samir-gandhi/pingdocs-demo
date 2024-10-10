# Error Message - Could not validate the verification code
## Configuration
ID:  8gqiq4sagn

Type: CONNECTION 

CapabilityName: customErrorMessage

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Background Color | #ffc8c1ff | 

 




### Additional Properties
errorCode
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
        "url": "httpResponseCode",
        "data": "{{local.1vyzcyazgf.payload.error.httpResponseCode}}",
        "tooltip": "{{local.1vyzcyazgf.payload.error.httpResponseCode}}",
        "children": [
          {
            "text": "httpResponseCode"
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


errorMessage
 ```json 
[
  {
    "children": [
      {
        "text": "Failed to validate the verification code."
      },
      {
        "text": ""
      }
    ]
  }
]
```


errorReason
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
        "url": "details",
        "data": "{{local.1vyzcyazgf.payload.error.details}}",
        "tooltip": "{{local.1vyzcyazgf.payload.error.details}}",
        "children": [
          {
            "text": "details"
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
| [r8sc175hhf](./r8sc175hhf.md) |  |