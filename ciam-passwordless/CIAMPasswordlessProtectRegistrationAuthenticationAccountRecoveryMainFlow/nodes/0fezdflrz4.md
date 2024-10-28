# Node - string 
Go to Sign On Success
## Configuration
ID:  0fezdflrz4

Type: CONNECTION 

CapabilityName: goToNode

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- || Valid Authentication Method | json 
[
  {
    "children": [
      {
        "text": "rememberme"
      }
    ]
  }
]
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "teleport.svg",        "url": "userId",        "data": "{{local.powvchr4kr.payload.output.userId}}",        "tooltip": "{{local.powvchr4kr.payload.output.userId}}",        "children": [          {            "text": "userId"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Expire Authentication Token | json 
[
  {
    "children": [
      {
        "text": "rememberme"
      }
    ]
  }
] |





### Additional Properties
createSession
```json 
[
  {
    "children": [
      {
        "text": "false"
      }
    ]
  }
]
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
        "data": "{{local.icv9ot1nro.payload.output.matchedUser.email}}",
        "tooltip": "{{local.icv9ot1nro.payload.output.matchedUser.email}}",
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


flowMethod
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
        "url": "flowMethod",
        "data": "{{local.ins74ygtvc.payload.output.flowMethod}}",
        "tooltip": "{{local.ins74ygtvc.payload.output.flowMethod}}",
        "children": [
          {
            "text": "flowMethod"
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


nodeInstanceId
```string 
x8uq3h1ccd
```


pingOneUserId
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
        "url": "id",
        "data": "{{local.w16j6hvh6d.payload.output.session.user.id}}",
        "tooltip": "{{local.w16j6hvh6d.payload.output.session.user.id}}",
        "children": [
          {
            "text": "id"
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




