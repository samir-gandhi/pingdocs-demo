# Functions - Set Flow Variables
## Configuration
ID:  7yrdpb4c81

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
	const results = {};

	results["username"] = params.flowParameters.username;

	return { ...results };
}
```


outputSchema
 ```json 
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


variableInputList
 ```json 

```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
|  | [avwmu6hzfh](./avwmu6hzfh.md) |