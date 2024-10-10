# PingOne - Create the PingOne user
## Configuration
ID:  rx35m4y6sp

Type: CONNECTION 

CapabilityName: createUser

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Creates the PingOne account for the user | 
 




### Additional Properties
additionalUserProperties
 ```json 

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
        "data": "{{local.z876lbl7xg.payload.output.email}}",
        "tooltip": "{{local.z876lbl7xg.payload.output.email}}",
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
        "url": "lastName",
        "data": "{{local.lx6499vpt4.payload.output.lastName}}",
        "tooltip": "{{local.lx6499vpt4.payload.output.lastName}}",
        "children": [
          {
            "text": "lastName"
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
        "data": "{{local.lx6499vpt4.payload.output.firstName}}",
        "tooltip": "{{local.lx6499vpt4.payload.output.firstName}}",
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


lifecycleStatus
 ```json 
VERIFICATION_REQUIRED
```


password
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
        "url": "password",
        "data": "{{local.fuil2gnc5f.payload.output.password}}",
        "tooltip": "{{local.fuil2gnc5f.payload.output.password}}",
        "children": [
          {
            "text": "password"
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


passwordForCreateUser
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
        "url": "password",
        "data": "{{local.1ftyww4qrg.payload.output.password}}",
        "tooltip": "{{local.1ftyww4qrg.payload.output.password}}",
        "children": [
          {
            "text": "password"
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


population
 ```json 
useDefaultPopulation
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
        "src": "teleport.svg",
        "url": "populationId",
        "data": "{{local.qp6fpnw2hk.payload.output.populationId}}",
        "tooltip": "{{local.qp6fpnw2hk.payload.output.populationId}}",
        "children": [
          {
            "text": "populationId"
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
        "url": "email",
        "data": "{{local.z876lbl7xg.payload.output.email}}",
        "tooltip": "{{local.z876lbl7xg.payload.output.email}}",
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




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [updxs8x4oi](./updxs8x4oi.md) | [ocq1m14pys](./ocq1m14pys.md) |