# PingOne MFA - string 
Create MFA Device
## Configuration
ID:  8jrbqcts2g

Type: CONNECTION 

CapabilityName: createDevice

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "pingIdentity.svg",        "url": "id",        "data": "{{local.3y03qc0kxe.payload.output.matchedUser.id}}",        "tooltip": "{{local.3y03qc0kxe.payload.output.matchedUser.id}}",        "children": [          {            "text": "id"          }        ]      },      {        "text": ""      }    ]  }] ```| 






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
| Evaluator | [mtaqacdw1m](./mtaqacdw1m.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[hk00gx2f95](./hk00gx2f95.md) | 