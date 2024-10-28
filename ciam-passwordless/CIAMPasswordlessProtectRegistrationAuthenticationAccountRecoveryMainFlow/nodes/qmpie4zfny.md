# Functions - string 
Check if Known Device
## Configuration
ID:  qmpie4zfny

Type: CONNECTION 

CapabilityName: AEqualsB






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
        "src": "flow-connector.svg",
        "url": "ciam_protectDeviceStatus",
        "data": "{{local.mt49dyk6zx.payload.output.ciam_protectDeviceStatus}}",
        "tooltip": "{{local.mt49dyk6zx.payload.output.ciam_protectDeviceStatus}}",
        "children": [
          {
            "text": "ciam_protectDeviceStatus"
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
        "text": "KNOWN_DEVICE"
      }
    ]
  }
]
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [o0ebgiurvi](./o0ebgiurvi.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[gaj3ygo1j4](./gaj3ygo1j4.md) | 