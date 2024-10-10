# PingOne MFA - Activate Device
## Configuration
ID:  5863kwjvsw

Type: CONNECTION 

CapabilityName: activateDevice

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```[  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "pingIdentity.svg",        "url": "id",        "data": "{{local.flt9ewj1a9.payload.output.matchedUser.id}}",        "tooltip": "{{local.flt9ewj1a9.payload.output.matchedUser.id}}",        "children": [          {            "text": "id"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Node Description | Activate Device | 
 




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
 ```json 
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
 ```json 
ACTIVE
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [wb4u3n0g7a](./wb4u3n0g7a.md) | [oiy97ee3bv](./oiy97ee3bv.md) |