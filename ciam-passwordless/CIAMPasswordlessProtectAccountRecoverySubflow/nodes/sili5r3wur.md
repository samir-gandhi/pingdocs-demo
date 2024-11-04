# Node - string 
Go to Sign On Success
## Configuration
ID:  sili5r3wur

Type: CONNECTION 

CapabilityName: goToNode

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- || Valid Authentication Method | json 
[
  {
    "children": [
      {
        "text": "invalid"
      }
    ]
  }
]
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "pingIdentity.svg",        "url": "id",        "data": "{{local.0jvt7xvej2.payload.output.matchedUser.id}}",        "tooltip": "{{local.0jvt7xvej2.payload.output.matchedUser.id}}",        "children": [          {            "text": "id"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Expire Authentication Token | json 
[
  {
    "children": [
      {
        "text": "invalid"
      }
    ]
  }
] |





### Additional Properties
authMethod
```json 
[
  {
    "children": [
      {
        "text": "pwd"
      }
    ]
  }
]
```


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


nodeInstanceId
```string 
j3hvs9dks4
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
        "data": "{{local.p7gnqv4r4t.payload.output.passwordState.user.id}}",
        "tooltip": "{{local.p7gnqv4r4t.payload.output.passwordState.user.id}}",
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


sublfowResult
```json 
[
  {
    "children": [
      {
        "text": "complete"
      }
    ]
  }
]
```



