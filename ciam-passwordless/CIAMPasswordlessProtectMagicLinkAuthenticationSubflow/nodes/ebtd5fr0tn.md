# Challenge - string 
Approve Challenge Status
## Configuration
ID:  ebtd5fr0tn

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
```string 
approved
```


claimsNameValuePairs
```
```


isChallengeComplete
```bool 
false
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [v0rkta2j1x](./v0rkta2j1x.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator |[drn0tajuo1](./drn0tajuo1.md) | 