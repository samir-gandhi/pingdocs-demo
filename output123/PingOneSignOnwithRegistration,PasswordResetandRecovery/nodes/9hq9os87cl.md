# Error Message - Password update failed
## Configuration
ID:  9hq9os87cl

Type: action 

CapabilityName: customErrorMessage

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Received an error when trying to update the user&#39;s password in PingOne | }
 




### Additional Properties
errorCallbackSuppress
 ```json 
true
```


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
        "data": "{{local.0c41v9ejkb.payload.error.httpResponseCode}}",
        "tooltip": "{{local.0c41v9ejkb.payload.error.httpResponseCode}}",
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
        "text": "Failed to update the user&#39;s password"
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
        "data": "{{local.0c41v9ejkb.payload.error.code}}",
        "tooltip": "{{local.0c41v9ejkb.payload.error.code}}",
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
        "data": "{{local.0c41v9ejkb.payload.error.message}}",
        "tooltip": "{{local.0c41v9ejkb.payload.error.message}}",
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
        "data": "{{local.0c41v9ejkb.payload.error.details}}",
        "tooltip": "{{local.0c41v9ejkb.payload.error.details}}",
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



