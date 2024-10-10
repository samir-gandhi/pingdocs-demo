# Error Message - Check if MFA is Enabled.
## Configuration
ID:  rs2jbqnsry

Type: CONNECTION 

CapabilityName: customErrorMessage

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | This check is done from Passwordless user and hence MFA has to be enabled | 
 




### Additional Properties
errorCode
 ```json 
400
```


errorDescription
 ```json 
[
  {
    "children": [
      {
        "text": "An error has occurred. Contact Adminsitrator"
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
        "text": "Error"
      }
    ]
  }
]
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [fm7p6z4lgt](./fm7p6z4lgt.md) |  |