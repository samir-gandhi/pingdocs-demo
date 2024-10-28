# PingOne Authentication - string 
Redirect With Success Response
## Configuration
ID:  zlublpnvlp

Type: CONNECTION 

CapabilityName: returnSuccessResponseRedirect

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- || Valid Authentication Method | string 
useCustomAuthenticationMethods
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "teleport.svg",        "url": "pingOneUserId",        "data": "{{local.x8uq3h1ccd.payload.output.pingOneUserId}}",        "tooltip": "{{local.x8uq3h1ccd.payload.output.pingOneUserId}}",        "children": [          {            "text": "pingOneUserId"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Expire Authentication Token | string 
useCustomAuthenticationMethods |
| Node Background Color | html 
#9dc967ff | 






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

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [eum65le218](./eum65le218.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator |[o74snj74sy](./o74snj74sy.md) | 