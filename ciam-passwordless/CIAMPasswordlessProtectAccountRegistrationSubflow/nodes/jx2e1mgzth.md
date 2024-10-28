# Functions - string 
Adjust Auth Method
## Configuration
ID:  jx2e1mgzth

Type: CONNECTION 

CapabilityName: customFunction





### Output Schema
``` json 
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

### Additional Properties
code
```js 
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


variableInputList
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [vs1a4w3l05](./vs1a4w3l05.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[8tqp4g8v75](./8tqp4g8v75.md) | 