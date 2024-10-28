# PingOne - string 
Validate Password
## Configuration
ID:  us1sbucx0m

Type: CONNECTION 

CapabilityName: checkPassword

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| User ID |```json [  {    "children": [      {        "text": ""      },      {        "text": ""      },      {        "type": "link",        "src": "pingIdentity.svg",        "url": "id",        "data": "{{local.icv9ot1nro.payload.output.matchedUser.id}}",        "tooltip": "{{local.icv9ot1nro.payload.output.matchedUser.id}}",        "children": [          {            "text": "id"          }        ]      },      {        "text": ""      }    ]  }] ```| 

| Node Description | string 
Validates that the user submitted the correct password for the account associated with the username | 





### Additional Properties
checkPassword_localizedErrors
```
```


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
        "src": "pingIdentity.svg",
        "url": "id",
        "data": "{{local.t09lk8opxa.payload.output.matchedUser.id}}",
        "tooltip": "{{local.t09lk8opxa.payload.output.matchedUser.id}}",
        "children": [
          {
            "text": "id"
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


matchAttribute
```string 
id
```


password
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
        "url": "password",
        "data": "{{local.rstodi2zw1.payload.output.password}}",
        "tooltip": "{{local.rstodi2zw1.payload.output.password}}",
        "children": [
          {
            "text": "password"
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
| EVAL | [y7f4468q9f](./y7f4468q9f.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[c9kmm14iq0](./c9kmm14iq0.md) | 