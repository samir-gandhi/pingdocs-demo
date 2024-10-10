# Http - Send Error Response
## Configuration
ID:  hxmqf7sb52

Type: CONNECTION 

CapabilityName: createErrorResponse

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Background Color | #ffc8c1ff | 

 




### Additional Properties
claimsNameValuePairs
 ```json 

```


message
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
        "url": "error",
        "data": "{{local.b028sqws7r.payload.error}}",
        "tooltip": "{{local.b028sqws7r.payload.error}}",
        "children": [
          {
            "text": "error"
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
| [b900rty9pd](./b900rty9pd.md) |  |