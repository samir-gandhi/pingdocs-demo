# Flow Conductor - string 
Device Registration
## Configuration
ID:  d915blmeth

Type: CONNECTION 

CapabilityName: startUiSubFlow






### Additional Properties
allowCancel
```json 
[
  {
    "children": [
      {
        "text": "true"
      }
    ]
  }
]
```


allowedDeviceTypes
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
        "url": "flowAllowedDeviceTypes",
        "data": "{{local.61gkn04fvn.payload.output.flowAllowedDeviceTypes}}",
        "tooltip": "{{local.61gkn04fvn.payload.output.flowAllowedDeviceTypes}}",
        "children": [
          {
            "text": "flowAllowedDeviceTypes"
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


ciam_companyLogo
```html 
[
  {
    "children": [
      {
        "text": "<div class="dialog-content-header dialog-content__header" style="height: 85px"><div class="dialog-content-header__logo"></div></div>"
      }
    ]
  }
]
```


passwordlessRequired
```json 
[
  {
    "children": [
      {
        "text": "true"
      }
    ]
  }
]
```


pingOneUserId
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
        "url": "userId",
        "data": "{{local.61gkn04fvn.payload.output.userId}}",
        "tooltip": "{{local.61gkn04fvn.payload.output.userId}}",
        "children": [
          {
            "text": "userId"
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
| EVAL | [1lngxsfyuk](./1lngxsfyuk.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator |[17n6cajfer](./17n6cajfer.md) | 