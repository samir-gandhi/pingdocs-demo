# Node
## Configuration
ID:  h0rcajanl2

Type: CONNECTION 

CapabilityName: goToNode

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- || Valid Authentication Method | json 
[
  {
    "children": [
      {
        "text": "pwd"
      }
    ]
  }
]
| Expire Authentication Token | json 
[
  {
    "children": [
      {
        "text": "pwd"
      }
    ]
  }
] |





### Additional Properties
flowAgreementEnabled
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
        "url": "flowAgreementEnabled",
        "data": "{{local.el9cmscetd.payload.output.flowAgreementEnabled}}",
        "tooltip": "{{local.el9cmscetd.payload.output.flowAgreementEnabled}}",
        "children": [
          {
            "text": "flowAgreementEnabled"
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


flowAgreementId
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
        "url": "flowAgreementId",
        "data": "{{local.el9cmscetd.payload.output.flowAgreementId}}",
        "tooltip": "{{local.el9cmscetd.payload.output.flowAgreementId}}",
        "children": [
          {
            "text": "flowAgreementId"
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
        "data": "{{local.el9cmscetd.payload.output.flowMethod}}",
        "tooltip": "{{local.el9cmscetd.payload.output.flowMethod}}",
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


lifeCycleStatus
```json 
[
  {
    "children": [
      {
        "text": "ACCOUNT_OK"
      }
    ]
  }
]
```


nodeInstanceId
```string 
1r9qfce4ko
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
        "src": "auth.svg",
        "url": "p1UserId",
        "data": "{{global.p1UserId}}",
        "tooltip": "{{global.p1UserId}}",
        "children": [
          {
            "text": "p1UserId"
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


rememberMe
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




