# Functions - string 
Verify Passwords Match
## Configuration
ID:  16hlhgpr5h

Type: CONNECTION 

CapabilityName: customFunction

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
Verify new passwords match before setting | 




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
| EVAL | [fecpsdg3u3](./fecpsdg3u3.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| Evaluator |[9o0jtjpq4i](./9o0jtjpq4i.md) | 