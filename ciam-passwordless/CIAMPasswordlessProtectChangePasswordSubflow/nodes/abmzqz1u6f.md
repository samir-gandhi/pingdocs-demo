# Error Message - Invalid password
## Configuration
ID:  abmzqz1u6f

Type: CONNECTION 

CapabilityName: customErrorMessage

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | An error occurred while changing the password | 
 




### Additional Properties
errorCode
 ```json 
[
  {
    "children": [
      {
        "text": "Invalid"
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
        "text": ""
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
        "text": ""
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "functions.svg",
        "url": "updatedErrorMessage",
        "data": "{{local.okw0g6i84d.payload.output.updatedErrorMessage}}",
        "tooltip": "{{local.okw0g6i84d.payload.output.updatedErrorMessage}}",
        "children": [
          {
            "text": "updatedErrorMessage"
          }
        ]
      },
      {
        "text": ""
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
| [um3lcpaulo](./um3lcpaulo.md) |  |