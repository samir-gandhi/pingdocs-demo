# PingOne - Resend recovery code
## Configuration
ID:  rfwgqmb87x

Type: CONNECTION 

CapabilityName: sendRecoveryCode

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```[  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "pingIdentity.svg",        "url": "id",        "data": "{{local.0jvt7xvej2.payload.output.matchedUser.id}}",        "tooltip": "{{local.0jvt7xvej2.payload.output.matchedUser.id}}",        "children": [          {            "text": "id"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Node Description | Sends a password recovery OTP to user to verify they own this account | 
 




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
 ```json 

```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [t6hyz30ejn](./t6hyz30ejn.md) | [4mpcqubv22](./4mpcqubv22.md) |