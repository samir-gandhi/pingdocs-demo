# Functions - Which button was selected?
## Configuration
ID:  2bqi2hcyod

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
        "data": "{{local.fkekf3oi8e.payload.output.buttonValue}}",
        "tooltip": "{{local.fkekf3oi8e.payload.output.buttonValue}}",
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



