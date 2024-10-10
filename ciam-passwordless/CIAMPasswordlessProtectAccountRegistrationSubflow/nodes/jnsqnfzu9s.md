# Functions - Verify Passwords Match
## Configuration
ID:  jnsqnfzu9s

Type: CONNECTION 

CapabilityName: customFunction

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Verify new passwords match before setting | 
 




### Additional Properties
code
 ```json 
// Test to ensure passwords match
module.exports = a = async ({ params }) => {
	const password = params.password;
	const verifyPassword = params.verifyPassword;

	if (!password || !verifyPassword || (password !== verifyPassword)) {
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
| [kerq5fyp8w](./kerq5fyp8w.md) | [k0x7ywsse6](./k0x7ywsse6.md) |