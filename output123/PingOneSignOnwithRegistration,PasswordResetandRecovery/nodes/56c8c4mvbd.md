# Functions - Which button was selected?
## Configuration
ID:  56c8c4mvbd

Type: trigger 

CapabilityName: AEqualsMultipleB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Branch based on the button selected on the forgot password form | }
 




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
        "data": "{{local.qwnvng32z3.payload.output.buttonValue}}",
        "tooltip": "{{local.qwnvng32z3.payload.output.buttonValue}}",
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
        "text": "submit"
      }
    ]
  }
]
```


rightValueMultiple
 ```json 

```



