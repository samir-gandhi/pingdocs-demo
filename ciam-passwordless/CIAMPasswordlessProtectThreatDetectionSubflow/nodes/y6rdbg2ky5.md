# PingOne Protect - string 
Create PingOne Protect Risk with user and Environment details
## Configuration
ID:  y6rdbg2ky5

Type: CONNECTION 

CapabilityName: createRiskEvaluation

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "auth.svg",        "url": "userID",        "data": "{{global.parameters.userID}}",        "tooltip": "{{global.parameters.userID}}",        "children": [          {            "text": "userID"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Node Description | string 
Should have required variables to start the risk evaluation. | 





### Additional Properties
cookie
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
        "url": "usercookie",
        "data": "{{global.parameters.usercookie}}",
        "tooltip": "{{global.parameters.usercookie}}",
        "children": [
          {
            "text": "usercookie"
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


customAttributes
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
        "url": "customAttributes",
        "data": "{{global.parameters.customAttributes}}",
        "tooltip": "{{global.parameters.customAttributes}}",
        "children": [
          {
            "text": "customAttributes"
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


flowType
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
        "url": "flowType",
        "data": "{{global.parameters.flowType}}",
        "tooltip": "{{global.parameters.flowType}}",
        "children": [
          {
            "text": "flowType"
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


ipAddress
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
        "url": "ipAddress",
        "data": "{{global.parameters.ipAddress}}",
        "tooltip": "{{global.parameters.ipAddress}}",
        "children": [
          {
            "text": "ipAddress"
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


riskPolicySetId
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
        "url": "riskPolicyID",
        "data": "{{global.parameters.riskPolicyID}}",
        "tooltip": "{{global.parameters.riskPolicyID}}",
        "children": [
          {
            "text": "riskPolicyID"
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


sessionId
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
        "url": "SessionId",
        "data": "{{global.parameters.SessionId}}",
        "tooltip": "{{global.parameters.SessionId}}",
        "children": [
          {
            "text": "SessionId"
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


skRiskFP
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
        "url": "skriskcomponent",
        "data": "{{global.parameters.skriskcomponent}}",
        "tooltip": "{{global.parameters.skriskcomponent}}",
        "children": [
          {
            "text": "skriskcomponent"
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


targetResourceId
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
        "url": "applicationId",
        "data": "{{global.parameters.applicationId}}",
        "tooltip": "{{global.parameters.applicationId}}",
        "children": [
          {
            "text": "applicationId"
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


userAgent
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
        "url": "userAgent",
        "data": "{{global.parameters.userAgent}}",
        "tooltip": "{{global.parameters.userAgent}}",
        "children": [
          {
            "text": "userAgent"
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


userName
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
        "url": "userName",
        "data": "{{global.parameters.userName}}",
        "tooltip": "{{global.parameters.userName}}",
        "children": [
          {
            "text": "userName"
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


userType
```string 
PING_ONE
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [6b03psy0ol](./6b03psy0ol.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[vknqtnu7y2](./vknqtnu7y2.md) | 