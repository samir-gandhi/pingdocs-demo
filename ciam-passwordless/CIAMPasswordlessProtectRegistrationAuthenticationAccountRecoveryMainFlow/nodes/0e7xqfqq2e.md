# PingOne Authentication - Return With Success Response
## Configuration
ID:  0e7xqfqq2e

Type: CONNECTION 

CapabilityName: returnSuccessResponseWidget

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- || Valid Authentication Method | useCustomAuthenticationMethods
| User ID |```[  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "pingIdentity.svg",        "url": "id",        "data": "{{local.jimu9wsyls.payload.output.matchedUser.id}}",        "tooltip": "{{local.jimu9wsyls.payload.output.matchedUser.id}}",        "children": [          {            "text": "id"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Expire Authentication Token | useCustomAuthenticationMethods |
| Node Background Color | #9dc967ff | 

 




### Additional Properties
additionalProperties
 ```json 

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
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [jio5trsqxr](./jio5trsqxr.md) | [69tmgilhek](./69tmgilhek.md) |