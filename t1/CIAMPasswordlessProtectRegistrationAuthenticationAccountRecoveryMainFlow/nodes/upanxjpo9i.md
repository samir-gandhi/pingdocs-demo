# Node
## Configuration
ID:  upanxjpo9i

Type: CONNECTION 

CapabilityName: goToNode

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- || Valid Authentication Method | json 
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
        "url": "ciam_authMethod",
        "data": "{{global.variables.ciam_authMethod}}",
        "tooltip": "{{global.variables.ciam_authMethod}}",
        "children": [
          {
            "text": "ciam_authMethod"
          }
        ]
      },
      {
        "text": ""
      }
    ]
  }
]
| Expire Authentication Token | json 
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
        "url": "ciam_authMethod",
        "data": "{{global.variables.ciam_authMethod}}",
        "tooltip": "{{global.variables.ciam_authMethod}}",
        "children": [
          {
            "text": "ciam_authMethod"
          }
        ]
      },
      {
        "text": ""
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
        "text": ""
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "teleport.svg",
        "url": "createSession",
        "data": "{{local.1r9qfce4ko.payload.output.createSession}}",
        "tooltip": "{{local.1r9qfce4ko.payload.output.createSession}}",
        "children": [
          {
            "text": "createSession"
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
        "data": "{{local.1r9qfce4ko.payload.output.flowMethod}}",
        "tooltip": "{{local.1r9qfce4ko.payload.output.flowMethod}}",
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
        "src": "teleport.svg",
        "url": "pingOneUserId",
        "data": "{{local.1r9qfce4ko.payload.output.pingOneUserId}}",
        "tooltip": "{{local.1r9qfce4ko.payload.output.pingOneUserId}}",
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




