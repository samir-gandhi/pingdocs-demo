# PingOne MFA - Create OTP Device
## Configuration
ID:  pjzv5pikab

Type: CONNECTION 

CapabilityName: createDevice

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```[  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "auth.svg",        "url": "pingOneUserId",        "data": "{{global.parameters.pingOneUserId}}",        "tooltip": "{{global.parameters.pingOneUserId}}",        "children": [          {            "text": "pingOneUserId"          }        ]      },      {        "text": ""      }    ]  }] ```| 

 




### Additional Properties
customDeviceType
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
        "src": "teleport.svg",
        "url": "deviceType",
        "data": "{{local.dc2mhwx86e.payload.output.deviceType}}",
        "tooltip": "{{local.dc2mhwx86e.payload.output.deviceType}}",
        "children": [
          {
            "text": "deviceType"
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
enterDeviceType
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
        "text": ""
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "teleport.svg",
        "url": "email",
        "data": "{{local.dc2mhwx86e.payload.output.email}}",
        "tooltip": "{{local.dc2mhwx86e.payload.output.email}}",
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


phone
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
        "text": ""
      },
      {
        "text": ""
      },
      {
        "text": ""
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "teleport.svg",
        "url": "phone",
        "data": "{{local.dc2mhwx86e.payload.output.phone}}",
        "tooltip": "{{local.dc2mhwx86e.payload.output.phone}}",
        "children": [
          {
            "text": "phone"
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
ACTIVATION_REQUIRED
```


workforceDeviceType
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
        "text": ""
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "http.svg",
        "url": "buttonValue",
        "data": "{{local.m0hxpev7nt.payload.output.buttonValue}}",
        "tooltip": "{{local.m0hxpev7nt.payload.output.buttonValue}}",
        "children": [
          {
            "text": "buttonValue"
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
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [9a49qb1y7k](./9a49qb1y7k.md) | [thtxgh5tye](./thtxgh5tye.md) |