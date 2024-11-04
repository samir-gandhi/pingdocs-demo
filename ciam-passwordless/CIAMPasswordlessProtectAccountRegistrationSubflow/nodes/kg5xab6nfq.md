# Functions - string 
Verify Passwords Match
## Configuration
ID:  kg5xab6nfq

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
	const password = params.password;
	const verifyPassword = params.verifyPassword;

	if (!password || !verifyPassword || (password !== verifyPassword)) {
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
| EVAL | [daxhwjbxh3](./daxhwjbxh3.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[updxs8x4oi](./updxs8x4oi.md) | 