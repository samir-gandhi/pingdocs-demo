# Error Message - Could not validate the verification code
## Configuration
ID:  o6sr4tiubd

Type: action 

CapabilityName: customErrorMessage

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Background Color | #ffc8c1ff | 

| Node Description | Failed to validate the submitted verification code | }
 




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
        "data": "{{local.jw8ez5s8p8.payload.error.httpResponseCode}}",
        "tooltip": "{{local.jw8ez5s8p8.payload.error.httpResponseCode}}",
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


errorDescription
 ```json 
[
  {
    "children": [
      {
        "text": "Failed to validate the verification code"
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
        "text": ""
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "pingIdentity.svg",
        "url": "code",
        "data": "{{local.jw8ez5s8p8.payload.error.code}}",
        "tooltip": "{{local.jw8ez5s8p8.payload.error.code}}",
        "children": [
          {
            "text": "code"
          }
        ]
      },
      {
        "text": " "
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "pingIdentity.svg",
        "url": "message",
        "data": "{{local.jw8ez5s8p8.payload.error.message}}",
        "tooltip": "{{local.jw8ez5s8p8.payload.error.message}}",
        "children": [
          {
            "text": "message"
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
        "data": "{{local.jw8ez5s8p8.payload.error.details}}",
        "tooltip": "{{local.jw8ez5s8p8.payload.error.details}}",
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



