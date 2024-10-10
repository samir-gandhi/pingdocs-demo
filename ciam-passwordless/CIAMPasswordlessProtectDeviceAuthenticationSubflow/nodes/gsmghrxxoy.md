# Functions - Check for KNOWN DEVICE
## Configuration
ID:  gsmghrxxoy

Type: CONNECTION 

CapabilityName: AEqualsB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




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
        "data": "{{local.u9ab712lfx.payload.output.ciam_protectDeviceStatus}}",
        "tooltip": "{{local.u9ab712lfx.payload.output.ciam_protectDeviceStatus}}",
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
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [u22hch23vs](./u22hch23vs.md) | [nl0cxyid0x](./nl0cxyid0x.md) |