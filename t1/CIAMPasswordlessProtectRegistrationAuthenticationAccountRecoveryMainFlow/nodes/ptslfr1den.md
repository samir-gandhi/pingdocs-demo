# Functions - string 
Check if user can authenticate
## Configuration
ID:  ptslfr1den

Type: CONNECTION 

CapabilityName: AEqualsB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
Check if user can authenticate  | 





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
        "url": "canAuthenticate",
        "data": "{{local.eq6oq9q1ag.payload.output.matchedUser.account.canAuthenticate}}",
        "tooltip": "{{local.eq6oq9q1ag.payload.output.matchedUser.account.canAuthenticate}}",
        "children": [
          {
            "text": "canAuthenticate"
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
```string 
boolean
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator | [5gz6jcxdng](./5gz6jcxdng.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator |[dfcr1art1l](./dfcr1art1l.md) | 