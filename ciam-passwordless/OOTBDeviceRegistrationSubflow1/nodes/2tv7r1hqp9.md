# Functions - string 
Can User Register Another Device?
## Configuration
ID:  2tv7r1hqp9

Type: CONNECTION 

CapabilityName: ALessThanB






### Additional Properties
leftValueA
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
        "url": "size",
        "data": "{{local.te6t0zwohr.payload.output.rawResponse.size}}",
        "tooltip": "{{local.te6t0zwohr.payload.output.rawResponse.size}}",
        "children": [
          {
            "text": "size"
          }
        ]
      },
      {
        "text": ""
      },
      {
        "text": ""
      },
      {
        "text": ""
      },
      {
        "text": ""
      },
      {
        "text": ""
      },
      {
        "text": ""
      },
      {
        "text": ""
      },
      {
        "text": ""
      }
    ]
  },
  {
    "children": [
      {
        "text": ""
      }
    ]
  },
  {
    "children": [
      {
        "text": ""
      }
    ]
  }
]
```


rightValueB
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
        "url": "maxAllowedDevices",
        "data": "{{local.te6t0zwohr.payload.output.rawResponse._embedded.mfaSettings.pairing.maxAllowedDevices}}",
        "tooltip": "{{local.te6t0zwohr.payload.output.rawResponse._embedded.mfaSettings.pairing.maxAllowedDevices}}",
        "children": [
          {
            "text": "maxAllowedDevices"
          }
        ]
      },
      {
        "text": ""
      },
      {
        "text": ""
      }
    ]
  }
]
```


type
```string 
number
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [jh39me4hnk](./jh39me4hnk.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator |[qj3vhzekmd](./qj3vhzekmd.md) | 