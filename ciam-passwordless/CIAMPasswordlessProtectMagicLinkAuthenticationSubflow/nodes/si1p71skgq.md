# Challenge - Deny Challenge After Expiration
## Configuration
ID:  si1p71skgq

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
        "data": "{{local.zsk0ny89ud.payload.output.challenge}}",
        "tooltip": "{{local.zsk0ny89ud.payload.output.challenge}}",
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
denied
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [3ma220y2v8](./3ma220y2v8.md) | [rbbahd8wkk](./rbbahd8wkk.md) |