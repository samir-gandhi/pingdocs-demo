# PingOne MFA - string 
Start MFA Authentication
## Configuration
ID:  10oaokas61

Type: CONNECTION 

CapabilityName: createDeviceAuthentication

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "auth.svg",        "url": "pingOneUserId",        "data": "{{global.parameters.pingOneUserId}}",        "tooltip": "{{global.parameters.pingOneUserId}}",        "children": [          {            "text": "pingOneUserId"          }        ]      },      {        "text": ""      },      {        "text": ""      }    ]  }] ```| 






### Additional Properties
authTemplateName
```
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

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [0sua91hqk7](./0sua91hqk7.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator |[4l39ap532m](./4l39ap532m.md) | 