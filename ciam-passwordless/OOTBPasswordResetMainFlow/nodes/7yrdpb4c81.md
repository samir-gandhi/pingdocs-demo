# Functions - string 
Set Flow Variables
## Configuration
ID:  7yrdpb4c81

Type: CONNECTION 

CapabilityName: customFunction





### Output Schema
``` json 
{
	"output": {
		"type": "object",
		"properties": {
			"username": {
				"type": "boolean"
			},
			"flowAllowedDeviceTypes": {
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
	const results = {};

	results["username"] = params.flowParameters.username;

	return { ...results };
}
```


variableInputList
```
```




