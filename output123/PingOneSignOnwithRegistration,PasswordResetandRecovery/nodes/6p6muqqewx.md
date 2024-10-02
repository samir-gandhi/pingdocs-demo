# Functions - Check Password Status
## Configuration
ID:  6p6muqqewx

Type: trigger 

CapabilityName: AEqualsMultipleB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Branches based on the password status returned by PingOne | }
 




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
        "url": "status",
        "data": "{{local.dnu7jt3sjz.payload.output.rawResponse.status}}",
        "tooltip": "{{local.dnu7jt3sjz.payload.output.rawResponse.status}}",
        "children": [
          {
            "text": "status"
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


rightValueMultiple
 ```json 

```



