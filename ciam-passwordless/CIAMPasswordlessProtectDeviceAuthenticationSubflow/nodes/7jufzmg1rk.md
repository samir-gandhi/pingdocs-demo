# PingOne MFA - string 
Activate MFA Device
## Configuration
ID:  7jufzmg1rk

Type: CONNECTION 

CapabilityName: activateDevice

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "pingIdentity.svg",        "url": "id",        "data": "{{local.3y03qc0kxe.payload.output.matchedUser.id}}",        "tooltip": "{{local.3y03qc0kxe.payload.output.matchedUser.id}}",        "children": [          {            "text": "id"          }        ]      },      {        "text": ""      }    ]  }] ```| 






### Additional Properties
customDeviceType
```json 
{}
```


customNotificationPolicyId
```json 
{}
```


customTemplateVariant
```json 
{}
```


deviceId
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
        "data": "{{local.8jrbqcts2g.payload.output.rawResponse.id}}",
        "tooltip": "{{local.8jrbqcts2g.payload.output.rawResponse.id}}",
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


deviceType
```string 
EMAIL
```


email
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
        "url": "email",
        "data": "{{local.3y03qc0kxe.payload.output.matchedUser.email}}",
        "tooltip": "{{local.3y03qc0kxe.payload.output.matchedUser.email}}",
        "children": [
          {
            "text": "email"
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


otp
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
        "url": "passcode",
        "data": "{{local.onogvjusk6.payload.output.passcode}}",
        "tooltip": "{{local.onogvjusk6.payload.output.passcode}}",
        "children": [
          {
            "text": "passcode"
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


status
```string 
ACTIVE
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator | [kho2rpwvb7](./kho2rpwvb7.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[qw4n733f3t](./qw4n733f3t.md) | 