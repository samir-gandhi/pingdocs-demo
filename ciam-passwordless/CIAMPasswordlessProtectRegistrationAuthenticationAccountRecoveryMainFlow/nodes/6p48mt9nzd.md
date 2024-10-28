# Node
## Configuration
ID:  6p48mt9nzd

Type: CONNECTION 

CapabilityName: goToNode

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- || Valid Authentication Method | json 
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
        "url": "ciam_authMethod",
        "data": "{{local.7y41qu33vz.payload.output.ciam_authMethod}}",
        "tooltip": "{{local.7y41qu33vz.payload.output.ciam_authMethod}}",
        "children": [
          {
            "text": "ciam_authMethod"
          }
        ]
      },
      {
        "text": ""
      }
    ]
  }
]
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "flow-connector.svg",        "url": "ciam_pingOneUserId",        "data": "{{local.yuc5xfay4j.payload.output.ciam_pingOneUserId}}",        "tooltip": "{{local.yuc5xfay4j.payload.output.ciam_pingOneUserId}}",        "children": [          {            "text": "ciam_pingOneUserId"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Expire Authentication Token | json 
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
        "url": "ciam_authMethod",
        "data": "{{local.7y41qu33vz.payload.output.ciam_authMethod}}",
        "tooltip": "{{local.7y41qu33vz.payload.output.ciam_authMethod}}",
        "children": [
          {
            "text": "ciam_authMethod"
          }
        ]
      },
      {
        "text": ""
      }
    ]
  }
] |





### Additional Properties
createSession
```json 
[
  {
    "children": [
      {
        "text": "false"
      }
    ]
  }
]
```


flowMethod
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
        "src": "teleport.svg",
        "url": "flowMethod",
        "data": "{{local.el9cmscetd.payload.output.flowMethod}}",
        "tooltip": "{{local.el9cmscetd.payload.output.flowMethod}}",
        "children": [
          {
            "text": "flowMethod"
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


nodeInstanceId
```string 
x8uq3h1ccd
```


pingOneUserId
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
        "url": "ciam_pingOneUserId",
        "data": "{{local.7y41qu33vz.payload.output.ciam_pingOneUserId}}",
        "tooltip": "{{local.7y41qu33vz.payload.output.ciam_pingOneUserId}}",
        "children": [
          {
            "text": "ciam_pingOneUserId"
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




