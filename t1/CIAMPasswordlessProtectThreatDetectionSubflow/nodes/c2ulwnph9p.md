# Functions - string 
Detect Threat
## Configuration
ID:  c2ulwnph9p

Type: CONNECTION 

CapabilityName: arrayOfAIncludesB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
Check if PingOne protect has detected a BOT or AITM attack | 





### Additional Properties
leftValueA
```json 
[
  {
    "children": [
      {
        "text": "["BOT_MITIGATION","AITM_MITIGATION","TEMP_EMAIL_MITIGATION"]"
      },
      {
        "text": ""
      },
      {
        "text": ""
      },
      {
        "text": ""
      },
      {
        "text": ""
      },
      {
        "text": ""
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
        "text": ""
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "pingIdentity.svg",
        "url": "recommendedAction",
        "data": "{{local.y6rdbg2ky5.payload.output.rawResponse.result.recommendedAction}}",
        "tooltip": "{{local.y6rdbg2ky5.payload.output.rawResponse.result.recommendedAction}}",
        "children": [
          {
            "text": "recommendedAction"
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
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [vknqtnu7y2](./vknqtnu7y2.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator |[uizc04ybxq](./uizc04ybxq.md) | 