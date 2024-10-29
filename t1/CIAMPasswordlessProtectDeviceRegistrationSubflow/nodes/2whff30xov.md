# Functions - string 
Mask Email Address
## Configuration
ID:  2whff30xov

Type: CONNECTION 

CapabilityName: customFunction





### Output Schema
``` json 
{
	"output": {
		"type": "object",
		"properties": {
			"maskedEmail": {
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
	let email = params.email

	if (email) {
		const [username, domain] = email.split("@");
  		const maskedUsername =
    	username.charAt(0) &#43; "*".repeat(username.length - 2) &#43; username.slice(-1);
		email = maskedUsername &#43; "@" &#43; domain;
	}

	return {&#39;maskedEmail&#39;: email}
}
```


variableInputList
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [k9rrvndxtf](./k9rrvndxtf.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[h2d7rovpq5](./h2d7rovpq5.md) | 