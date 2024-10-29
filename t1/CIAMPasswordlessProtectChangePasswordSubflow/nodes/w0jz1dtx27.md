# Functions - string 
Verify Passwords Match
## Configuration
ID:  w0jz1dtx27

Type: CONNECTION 

CapabilityName: customFunction





### Output Schema
``` json 
{
	"output": {
		"type": "object",
		"properties": {
			"success": {
				"type": "string"
			}
		}
	}
} 
```

### Additional Properties
code
```js 
// Test to ensure passwords match
module.exports = a = async ({ params }) => {
	const newPassword = params.newPassword;
	const verifyNewPassword = params.verifyNewPassword;

	if (!newPassword || !verifyNewPassword || (newPassword !== verifyNewPassword)) {
		return false;
	}

	return { "success": true};
}
```


variableInputList
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [2inl0soj3i](./2inl0soj3i.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator |[6oeo7c9bch](./6oeo7c9bch.md) | 