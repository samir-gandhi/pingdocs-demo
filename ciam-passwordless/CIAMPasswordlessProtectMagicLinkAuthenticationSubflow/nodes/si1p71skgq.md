# Challenge - string 
Deny Challenge After Expiration
## Configuration
ID:  si1p71skgq

Type: CONNECTION 

CapabilityName: updateChallenge






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
```string 
denied
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [3ma220y2v8](./3ma220y2v8.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[rbbahd8wkk](./rbbahd8wkk.md) | 