# PingOne - Create the PingOne user
## Configuration
ID:  agjdg5vxr2

Type: action 

CapabilityName: createUser

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Creates the PingOne account for the user | }
 




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
        "data": "{{local.4dth5sn269.payload.output.email}}",
        "tooltip": "{{local.4dth5sn269.payload.output.email}}",
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
        "data": "{{local.4dth5sn269.payload.output.lastName}}",
        "tooltip": "{{local.4dth5sn269.payload.output.lastName}}",
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
        "data": "{{local.4dth5sn269.payload.output.firstName}}",
        "tooltip": "{{local.4dth5sn269.payload.output.firstName}}",
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
        "data": "{{local.4dth5sn269.payload.output.password}}",
        "tooltip": "{{local.4dth5sn269.payload.output.password}}",
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
        "data": "{{local.4dth5sn269.payload.output.email}}",
        "tooltip": "{{local.4dth5sn269.payload.output.email}}",
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



