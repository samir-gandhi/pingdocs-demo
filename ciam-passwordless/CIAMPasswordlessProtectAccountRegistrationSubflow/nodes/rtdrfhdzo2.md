# PingOne - string 
Set Account Password
## Configuration
ID:  rtdrfhdzo2

Type: CONNECTION 

CapabilityName: setPassword






### Additional Properties
identifier
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
        "url": "pingOneUserId",
        "data": "{{local.qnljz2ats7.payload.output.pingOneUserId}}",
        "tooltip": "{{local.qnljz2ats7.payload.output.pingOneUserId}}",
        "children": [
          {
            "text": "pingOneUserId"
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


passwordValue
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
        "data": "{{local.gnh7rkcsg6.payload.output.password}}",
        "tooltip": "{{local.gnh7rkcsg6.payload.output.password}}",
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





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [k0x7ywsse6](./k0x7ywsse6.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator |[5rnhpdt5er](./5rnhpdt5er.md) | 