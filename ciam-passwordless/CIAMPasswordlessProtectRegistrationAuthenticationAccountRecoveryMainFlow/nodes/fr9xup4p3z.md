# PingOne MFA - string 
Create Device
## Configuration
ID:  fr9xup4p3z

Type: CONNECTION 

CapabilityName: createDevice

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "pingIdentity.svg",        "url": "id",        "data": "{{local.flt9ewj1a9.payload.output.matchedUser.id}}",        "tooltip": "{{local.flt9ewj1a9.payload.output.matchedUser.id}}",        "children": [          {            "text": "id"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Node Description | string 
Create Device | 





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


notificationPolicyId
```string 
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
```string 
oneTime
```


status
```string 
ACTIVATION_REQUIRED
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator | [opojvoak73](./opojvoak73.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[3e3ddhe5la](./3e3ddhe5la.md) | 