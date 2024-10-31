# PingOne - string 
Find User
## Configuration
ID:  n6qy3v9bsy

Type: CONNECTION 

CapabilityName: userLookup






### Additional Properties
additionalUserProperties
```
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
        "src": "http.svg",
        "url": "email",
        "data": "{{local.howu8n9hsc.payload.output.email}}",
        "tooltip": "{{local.howu8n9hsc.payload.output.email}}",
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


family
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
        "src": "http.svg",
        "url": "secondName",
        "data": "{{local.howu8n9hsc.payload.output.secondName}}",
        "tooltip": "{{local.howu8n9hsc.payload.output.secondName}}",
        "children": [
          {
            "text": "secondName"
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


given
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
        "src": "http.svg",
        "url": "firstName",
        "data": "{{local.howu8n9hsc.payload.output.firstName}}",
        "tooltip": "{{local.howu8n9hsc.payload.output.firstName}}",
        "children": [
          {
            "text": "firstName"
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


matchAttributes
```
```


populationId
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
        "src": "variable.svg",
        "url": "registartionPopulationId",
        "data": "{{global.variables.registartionPopulationId}}",
        "tooltip": "{{global.variables.registartionPopulationId}}",
        "children": [
          {
            "text": "registartionPopulationId"
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


userIdentifierForFindUser
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
        "url": "email",
        "data": "{{global.parameters.email}}",
        "tooltip": "{{global.parameters.email}}",
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


username
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
        "src": "http.svg",
        "url": "username",
        "data": "{{local.howu8n9hsc.payload.output.username}}",
        "tooltip": "{{local.howu8n9hsc.payload.output.username}}",
        "children": [
          {
            "text": "username"
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




