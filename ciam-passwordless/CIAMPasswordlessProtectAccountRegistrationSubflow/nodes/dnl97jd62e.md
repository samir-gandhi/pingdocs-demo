# PingOne - js 
Create the PingOne user (Passwordless)
## Configuration
ID:  dnl97jd62e

Type: CONNECTION 

CapabilityName: createUser

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
Creates the PingOne account for the user | 





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
```string 
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


population
```string 
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

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [za37tpd5ja](./za37tpd5ja.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[3759wy9sgr](./3759wy9sgr.md) | 