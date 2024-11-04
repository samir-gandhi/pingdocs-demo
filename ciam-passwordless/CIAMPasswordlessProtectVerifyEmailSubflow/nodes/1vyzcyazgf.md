# PingOne - string 
Validate verification code
## Configuration
ID:  1vyzcyazgf

Type: CONNECTION 

CapabilityName: verifyEmail

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
Sends the verification code to PingOne to validate | 





### Additional Properties
identifier
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
        "src": "auth.svg",
        "url": "pingOneUserId",
        "data": "{{global.parameters.pingOneUserId}}",
        "tooltip": "{{global.parameters.pingOneUserId}}",
        "children": [
          {
            "text": "pingOneUserId"
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


verificationCode
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
        "src": "http.svg",
        "url": "verificationCode",
        "data": "{{local.s5yykzv8zd.payload.output.verificationCode}}",
        "tooltip": "{{local.s5yykzv8zd.payload.output.verificationCode}}",
        "children": [
          {
            "text": "verificationCode"
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

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [hpve55zazv](./hpve55zazv.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[r8sc175hhf](./r8sc175hhf.md) | 