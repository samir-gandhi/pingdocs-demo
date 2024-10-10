# Functions - Check if Known Device
## Configuration
ID:  qmpie4zfny

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
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [o0ebgiurvi](./o0ebgiurvi.md) | [gaj3ygo1j4](./gaj3ygo1j4.md) |