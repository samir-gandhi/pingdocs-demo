# Functions - Update Error Message
## Configuration
ID:  f93pbyvrj2

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
	let errorMessage = params.errorMessage;

	if (errorMessage === "phone: must be a well-formed phone number with a valid country code followed by a phone number") {
		errorMessage = "Enter a valid phone number, including the country code.";
	}

	return {&#39;updatedErrorMessage&#39;: errorMessage};
}
```


outputSchema
 ```json 
{
	"output": {
		"type": "object",
		"properties": {
			"updatedErrorMessage": {
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
| [2my7xaouma](./2my7xaouma.md) | [hqdb3y3i65](./hqdb3y3i65.md) |