# Functions - Verify User Found
## Configuration
ID:  k92l3sshiz

Type: trigger 

CapabilityName: customFunction

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




### Additional Properties
checkNullORUndefined
 ```json 
true
```


code
 ```json 
module.exports = a = async ({params}) => {
	let userId = params.userId;

	if (! userId) {
		return false;
	}

	return 
}
```


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
        "src": "variable.svg",
        "url": "populationId",
        "data": "{{global.variables.populationId}}",
        "tooltip": "{{global.variables.populationId}}",
        "children": [
          {
            "text": "populationId"
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


variableInputList
 ```json 

```



