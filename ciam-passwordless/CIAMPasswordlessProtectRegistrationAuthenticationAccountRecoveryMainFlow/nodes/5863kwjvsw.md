# PingOne MFA - string 
Activate Device
## Configuration
ID:  5863kwjvsw

Type: CONNECTION 

CapabilityName: activateDevice

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "pingIdentity.svg",        "url": "id",        "data": "{{local.flt9ewj1a9.payload.output.matchedUser.id}}",        "tooltip": "{{local.flt9ewj1a9.payload.output.matchedUser.id}}",        "children": [          {            "text": "id"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Node Description | string 
Activate Device | 





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
        "data": "{{local.fr9xup4p3z.payload.output.rawResponse.id}}",
        "tooltip": "{{local.fr9xup4p3z.payload.output.rawResponse.id}}",
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
        "data": "{{local.flt9ewj1a9.payload.output.matchedUser.email}}",
        "tooltip": "{{local.flt9ewj1a9.payload.output.matchedUser.email}}",
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
        "data": "{{local.79cmhtu9fy.payload.output.passcode}}",
        "tooltip": "{{local.79cmhtu9fy.payload.output.passcode}}",
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
| Evaluator | [wb4u3n0g7a](./wb4u3n0g7a.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[oiy97ee3bv](./oiy97ee3bv.md) | 