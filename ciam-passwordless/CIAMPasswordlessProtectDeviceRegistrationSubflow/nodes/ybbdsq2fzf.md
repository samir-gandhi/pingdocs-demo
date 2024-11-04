# PingOne MFA - string 
Create device
## Configuration
ID:  ybbdsq2fzf

Type: CONNECTION 

CapabilityName: createDevice

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "auth.svg",        "url": "pingOneUserId",        "data": "{{global.parameters.pingOneUserId}}",        "tooltip": "{{global.parameters.pingOneUserId}}",        "children": [          {            "text": "pingOneUserId"          }        ]      },      {        "text": ""      }    ]  }] ```| 






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
        "data": "{{local.eh45uuo9ep.payload.output.deviceType}}",
        "tooltip": "{{local.eh45uuo9ep.payload.output.deviceType}}",
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
```string 
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
        "data": "{{local.eh45uuo9ep.payload.output.email}}",
        "tooltip": "{{local.eh45uuo9ep.payload.output.email}}",
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
        "url": "countryCode",
        "data": "{{local.eh45uuo9ep.payload.output.countryCode}}",
        "tooltip": "{{local.eh45uuo9ep.payload.output.countryCode}}",
        "children": [
          {
            "text": "countryCode"
          }
        ]
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
        "data": "{{local.eh45uuo9ep.payload.output.phone}}",
        "tooltip": "{{local.eh45uuo9ep.payload.output.phone}}",
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
```string 
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
        "type": "moustache",
        "data": "{{local.m0hxpev7nt.payload.output.buttonValue}}",
        "name": "buttonValue",
        "children": [
          {
            "text": ""
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
| EVAL | [wdmeq58d57](./wdmeq58d57.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[jozso5l9gu](./jozso5l9gu.md) | 