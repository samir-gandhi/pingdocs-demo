# PingOne MFA - Start MFA Authentication
## Configuration
ID:  10oaokas61

Type: CONNECTION 

CapabilityName: createDeviceAuthentication

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```[  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "auth.svg",        "url": "pingOneUserId",        "data": "{{global.parameters.pingOneUserId}}",        "tooltip": "{{global.parameters.pingOneUserId}}",        "children": [          {            "text": "pingOneUserId"          }        ]      },      {        "text": ""      },      {        "text": ""      }    ]  }] ```| 

 




### Additional Properties
authTemplateName
 ```json 

```


customApplicationId
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


fidoCompatibility
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
        "url": "webAuthenSupport",
        "data": "{{local.ek0byr7ikw.payload.output.webAuthenSupport}}",
        "tooltip": "{{local.ek0byr7ikw.payload.output.webAuthenSupport}}",
        "children": [
          {
            "text": "webAuthenSupport"
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


rpId
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
        "src": "variable.svg",
        "url": "rpid",
        "data": "{{global.variables.rpid}}",
        "tooltip": "{{global.variables.rpid}}",
        "children": [
          {
            "text": "rpid"
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
| [0sua91hqk7](./0sua91hqk7.md) | [4l39ap532m](./4l39ap532m.md) |