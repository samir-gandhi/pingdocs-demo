# Functions - Form Button Check
## Configuration
ID:  rjau0njx5i

Type: CONNECTION 

CapabilityName: AEqualsMultipleB

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
        "src": "http.svg",
        "url": "buttonValue",
        "data": "{{local.s5yykzv8zd.payload.output.buttonValue}}",
        "tooltip": "{{local.s5yykzv8zd.payload.output.buttonValue}}",
        "children": [
          {
            "text": "buttonValue"
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
        "text": "SUBMIT"
      }
    ]
  }
]
```


rightValueMultiple
 ```json 

```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [sju60xf677](./sju60xf677.md) | [t92nqcnwux](./t92nqcnwux.md), [n5icn97kyh](./n5icn97kyh.md) |