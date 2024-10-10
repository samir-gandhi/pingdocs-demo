# Error Customize - Password update failed
## Configuration
ID:  tfn7o3aug6

Type: CONNECTION 

CapabilityName: customErrorMessage

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




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
        "data": "{{local.mfmqkgj8ay.payload.error.httpResponseCode}}",
        "tooltip": "{{local.mfmqkgj8ay.payload.error.httpResponseCode}}",
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
        "text": "Failed to update your password"
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
        "text": ""
      },
      {
        "text": ""
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "pingIdentity.svg",
        "url": "message",
        "data": "{{local.7eaxdz9nwk.payload.error.message}}",
        "tooltip": "{{local.7eaxdz9nwk.payload.error.message}}",
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
        "data": "{{local.7eaxdz9nwk.payload.error.details}}",
        "tooltip": "{{local.7eaxdz9nwk.payload.error.details}}",
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
| [ateb0l10nl](./ateb0l10nl.md) |  |