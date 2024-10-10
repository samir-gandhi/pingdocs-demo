# PingOne MFA - Create Device
## Configuration
ID:  fr9xup4p3z

Type: CONNECTION 

CapabilityName: createDevice

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```[  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "pingIdentity.svg",        "url": "id",        "data": "{{local.flt9ewj1a9.payload.output.matchedUser.id}}",        "tooltip": "{{local.flt9ewj1a9.payload.output.matchedUser.id}}",        "children": [          {            "text": "id"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Node Description | Create Device | 
 




### Additional Properties
customApplicationId
 ```json 
{}
```


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


notificationPolicyId
 ```json 
6c9eb591-d8ea-4f90-8c04-8610e4f70203
```


oneTimeDeviceType
 ```json 
[
  {
    "children": [
      {
        "text": "EMAIL"
      }
    ]
  }
]
```


oneTimeEmailDevice
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


selectedDevice
 ```json 
oneTime
```


status
 ```json 
ACTIVATION_REQUIRED
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [opojvoak73](./opojvoak73.md) | [3e3ddhe5la](./3e3ddhe5la.md) |