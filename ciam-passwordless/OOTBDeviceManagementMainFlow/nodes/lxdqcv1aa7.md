# Functions - string 
Check If User Can Add New Device
## Configuration
ID:  lxdqcv1aa7

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
        "data": "{{local.4i8hh3qp83.payload.output.rawResponse.size}}",
        "tooltip": "{{local.4i8hh3qp83.payload.output.rawResponse.size}}",
        "children": [
          {
            "text": "size"
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
        "data": "{{local.4i8hh3qp83.payload.output.mfaSettings.pairing.maxAllowedDevices}}",
        "tooltip": "{{local.4i8hh3qp83.payload.output.mfaSettings.pairing.maxAllowedDevices}}",
        "children": [
          {
            "text": "maxAllowedDevices"
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


type
```string 
number
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [sjedcfzfgi](./sjedcfzfgi.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[vbk955oxjg](./vbk955oxjg.md) | 