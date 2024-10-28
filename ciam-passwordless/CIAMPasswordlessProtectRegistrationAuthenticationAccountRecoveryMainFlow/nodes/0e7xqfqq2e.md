# PingOne Authentication - string 
Return With Success Response
## Configuration
ID:  0e7xqfqq2e

Type: CONNECTION 

CapabilityName: returnSuccessResponseWidget

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- || Valid Authentication Method | string 
useCustomAuthenticationMethods
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "pingIdentity.svg",        "url": "id",        "data": "{{local.jimu9wsyls.payload.output.matchedUser.id}}",        "tooltip": "{{local.jimu9wsyls.payload.output.matchedUser.id}}",        "children": [          {            "text": "id"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Expire Authentication Token | string 
useCustomAuthenticationMethods |
| Node Background Color | html 
#9dc967ff | 






### Additional Properties
additionalProperties
```
```


customAuthenticationMethods
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
        "url": "authenticationMethods",
        "data": "{{local.x8uq3h1ccd.payload.output.authenticationMethods}}",
        "tooltip": "{{local.x8uq3h1ccd.payload.output.authenticationMethods}}",
        "children": [
          {
            "text": "authenticationMethods"
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
| EVAL | [jio5trsqxr](./jio5trsqxr.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator |[69tmgilhek](./69tmgilhek.md) | 