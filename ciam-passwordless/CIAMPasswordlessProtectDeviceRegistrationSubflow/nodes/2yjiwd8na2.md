# PingOne MFA - string 
Register User&#39;s Email As MFA Device
## Configuration
ID:  2yjiwd8na2

Type: CONNECTION 

CapabilityName: createDevice

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "auth.svg",        "url": "pingOneUserId",        "data": "{{global.parameters.pingOneUserId}}",        "tooltip": "{{global.parameters.pingOneUserId}}",        "children": [          {            "text": "pingOneUserId"          }        ]      },      {        "text": ""      }    ]  }] ```| 






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
        "src": "auth.svg",
        "url": "email",
        "data": "{{global.parameters.email}}",
        "tooltip": "{{global.parameters.email}}",
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


status
```string 
ACTIVE
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [zdzabypfcv](./zdzabypfcv.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator |[ltkdlim024](./ltkdlim024.md) | 