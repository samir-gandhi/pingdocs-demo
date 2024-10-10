# Node - Go to Sign On Success
## Configuration
ID:  gj8d9gmnwj

Type: CONNECTION 

CapabilityName: goToNode

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- || Valid Authentication Method | [
  {
    "children": [
      {
        "text": "pwd"
      }
    ]
  }
]
| User ID |```[  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "teleport.svg",        "url": "userId",        "data": "{{local.powvchr4kr.payload.output.userId}}",        "tooltip": "{{local.powvchr4kr.payload.output.userId}}",        "children": [          {            "text": "userId"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Expire Authentication Token | [
  {
    "children": [
      {
        "text": "pwd"
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
        "data": "{{local.powvchr4kr.payload.output.flowMethod}}",
        "tooltip": "{{local.powvchr4kr.payload.output.flowMethod}}",
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
 ```json 
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
        "src": "teleport.svg",
        "url": "pingOneUserId",
        "data": "{{local.powvchr4kr.payload.output.pingOneUserId}}",
        "tooltip": "{{local.powvchr4kr.payload.output.pingOneUserId}}",
        "children": [
          {
            "text": "pingOneUserId"
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
| [liu3llworn](./liu3llworn.md) |  |