# Functions - Verify Passwords Match
## Configuration
ID:  w0jz1dtx27

Type: CONNECTION 

CapabilityName: customFunction

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




### Additional Properties
code
 ```json 
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


outputSchema
 ```json 
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


variableInputList
 ```json 

```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [2inl0soj3i](./2inl0soj3i.md) | [6oeo7c9bch](./6oeo7c9bch.md) |