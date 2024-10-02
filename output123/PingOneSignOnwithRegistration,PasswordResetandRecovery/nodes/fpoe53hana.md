# Error Message - Failed to create the PingOne identity
## Configuration
ID:  fpoe53hana

Type: action 

CapabilityName: customErrorMessage

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Background Color | #ffc8c1ff | 

| Node Description | There was an error when trying to create the account in PingOne | }
 




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
        "data": "{{local.agjdg5vxr2.payload.error.httpResponseCode}}",
        "tooltip": "{{local.agjdg5vxr2.payload.error.httpResponseCode}}",
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
        "text": "There was an error when trying to create the account in PingOne"
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
        "data": "{{local.agjdg5vxr2.payload.error.code}}",
        "tooltip": "{{local.agjdg5vxr2.payload.error.code}}",
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
        "data": "{{local.agjdg5vxr2.payload.error.message}}",
        "tooltip": "{{local.agjdg5vxr2.payload.error.message}}",
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
        "data": "{{local.agjdg5vxr2.payload.error.details}}",
        "tooltip": "{{local.agjdg5vxr2.payload.error.details}}",
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



