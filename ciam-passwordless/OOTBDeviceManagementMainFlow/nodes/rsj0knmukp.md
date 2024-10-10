# Functions - Check If MFA Is enabled?
## Configuration
ID:  rsj0knmukp

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
        "src": "pingIdentity.svg",
        "url": "mfaEnabled",
        "data": "{{local.7rwri5u6ra.payload.output.matchedUser.mfaEnabled}}",
        "tooltip": "{{local.7rwri5u6ra.payload.output.matchedUser.mfaEnabled}}",
        "children": [
          {
            "text": "mfaEnabled"
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
        "text": "true"
      }
    ]
  }
]
```


type
 ```json 
boolean
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [rxrwt223m5](./rxrwt223m5.md) | [3jsczqq7hm](./3jsczqq7hm.md) |