# Functions - Detect Threat
## Configuration
ID:  c2ulwnph9p

Type: CONNECTION 

CapabilityName: arrayOfAIncludesB

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Check if PingOne protect has detected a BOT or AITM attack | 
 




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
 ```json 

```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [vknqtnu7y2](./vknqtnu7y2.md) | [uizc04ybxq](./uizc04ybxq.md) |