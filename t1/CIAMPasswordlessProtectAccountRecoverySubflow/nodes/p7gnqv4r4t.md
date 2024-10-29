# PingOne - string 
Set New Password
## Configuration
ID:  p7gnqv4r4t

Type: CONNECTION 

CapabilityName: recoverPassword

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "pingIdentity.svg",        "url": "id",        "data": "{{local.0jvt7xvej2.payload.output.matchedUser.id}}",        "tooltip": "{{local.0jvt7xvej2.payload.output.matchedUser.id}}",        "children": [          {            "text": "id"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Node Description | string 
Sets a new password if the user exists and the submitted recovery code is valid | 





### Additional Properties
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
        "src": "pingIdentity.svg",
        "url": "id",
        "data": "{{local.0jvt7xvej2.payload.output.matchedUser.id}}",
        "tooltip": "{{local.0jvt7xvej2.payload.output.matchedUser.id}}",
        "children": [
          {
            "text": "id"
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


newPassword
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
        "src": "http.svg",
        "url": "newPassword",
        "data": "{{local.h4u1as8yg4.payload.output.newPassword}}",
        "tooltip": "{{local.h4u1as8yg4.payload.output.newPassword}}",
        "children": [
          {
            "text": "newPassword"
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


recoverPassword_localizedErrors
```
```


recoveryCode
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
        "src": "http.svg",
        "url": "recoveryCode",
        "data": "{{local.h4u1as8yg4.payload.output.recoveryCode}}",
        "tooltip": "{{local.h4u1as8yg4.payload.output.recoveryCode}}",
        "children": [
          {
            "text": "recoveryCode"
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

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [1brhauigps](./1brhauigps.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[c6tyb3dxi1](./c6tyb3dxi1.md) | 