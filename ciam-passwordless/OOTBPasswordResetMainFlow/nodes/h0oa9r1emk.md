# Flow Conductor - Change Password
## Configuration
ID:  h0oa9r1emk

Type: CONNECTION 

CapabilityName: startUiSubFlow

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




### Additional Properties
ciam_companyLogo
 ```json 
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


showSuccessMessage
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


userID
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
        "url": "id",
        "data": "{{local.scja20ci5q.payload.output.matchedUser.id}}",
        "tooltip": "{{local.scja20ci5q.payload.output.matchedUser.id}}",
        "children": [
          {
            "text": "id"
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
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [zbtrq27f5e](./zbtrq27f5e.md) | [1xqdfym9yi](./1xqdfym9yi.md) |