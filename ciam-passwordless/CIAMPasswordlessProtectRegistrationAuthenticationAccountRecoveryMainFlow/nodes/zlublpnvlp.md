# PingOne Authentication - Redirect With Success Response
## Configuration
ID:  zlublpnvlp

Type: CONNECTION 

CapabilityName: returnSuccessResponseRedirect

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- || Valid Authentication Method | useCustomAuthenticationMethods
| User ID |```[  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "teleport.svg",        "url": "pingOneUserId",        "data": "{{local.x8uq3h1ccd.payload.output.pingOneUserId}}",        "tooltip": "{{local.x8uq3h1ccd.payload.output.pingOneUserId}}",        "children": [          {            "text": "pingOneUserId"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Expire Authentication Token | useCustomAuthenticationMethods |
| Node Background Color | #9dc967ff | 

 




### Additional Properties
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
| [eum65le218](./eum65le218.md) | [o74snj74sy](./o74snj74sy.md) |