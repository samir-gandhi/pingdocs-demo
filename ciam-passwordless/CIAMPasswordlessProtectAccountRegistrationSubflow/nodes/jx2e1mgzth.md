# Functions - Adjust Auth Method
## Configuration
ID:  jx2e1mgzth

Type: CONNECTION 

CapabilityName: customFunction

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




### Additional Properties
code
 ```json 
// Write your code here
// Supported language: Javascript 
module.exports = a = async ({params}) => {
	let authMethod = params.authMethod

	if (!authMethod.includes("email")) {
		authMethod = authMethod.concat(" email")
	}

	return {&#39;adjustedAuthMethod&#39;: authMethod}
}
```


outputSchema
 ```json 
{
	"output": {
		"type": "object",
		"properties": {
			"adjustedAuthMethod": {
				"type": "string"
			}
		}
	}
}
```


variableInputList
 ```json 

```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [vs1a4w3l05](./vs1a4w3l05.md) | [8tqp4g8v75](./8tqp4g8v75.md) |