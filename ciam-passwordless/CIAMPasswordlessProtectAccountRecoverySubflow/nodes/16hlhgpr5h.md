# Functions - Verify Passwords Match
## Configuration
ID:  16hlhgpr5h

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
| [fecpsdg3u3](./fecpsdg3u3.md) | [9o0jtjpq4i](./9o0jtjpq4i.md) |