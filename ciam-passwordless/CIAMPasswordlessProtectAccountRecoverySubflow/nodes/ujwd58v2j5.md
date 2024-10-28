# PingOne - string 
Send Recovery Code
## Configuration
ID:  ujwd58v2j5

Type: CONNECTION 

CapabilityName: sendRecoveryCode

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "pingIdentity.svg",        "url": "id",        "data": "{{local.0jvt7xvej2.payload.output.matchedUser.id}}",        "tooltip": "{{local.0jvt7xvej2.payload.output.matchedUser.id}}",        "children": [          {            "text": "id"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Node Description | string 
Sends a password recovery OTP to user to verify they own this account | 





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


sendRecoveryCode_localizedErrors
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [eph6l2tfnr](./eph6l2tfnr.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[n0ympwqzwl](./n0ympwqzwl.md) | 