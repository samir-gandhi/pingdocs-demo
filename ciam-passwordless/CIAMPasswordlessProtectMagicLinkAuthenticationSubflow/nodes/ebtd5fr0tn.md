# Challenge - Approve Challenge Status
## Configuration
ID:  ebtd5fr0tn

Type: CONNECTION 

CapabilityName: updateChallenge

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




### Additional Properties
challenge
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
        "url": "challenge",
        "data": "{{local.hhwhmetaid.payload.output.challenge}}",
        "tooltip": "{{local.hhwhmetaid.payload.output.challenge}}",
        "children": [
          {
            "text": "challenge"
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


challengeStatus
 ```json 
approved
```


claimsNameValuePairs
 ```json 

```


isChallengeComplete
 ```json 
false
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [v0rkta2j1x](./v0rkta2j1x.md) | [drn0tajuo1](./drn0tajuo1.md) |