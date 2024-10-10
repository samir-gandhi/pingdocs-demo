# Functions - Transform Passcode To Lowercase
## Configuration
ID:  r6lnkuy0yh

Type: CONNECTION 

CapabilityName: customFunction

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




### Additional Properties
code
 ```json 
module.exports = a = async ({ params }) => {
	const passcode = params.selectedDeviceType === "YUBIKEY" ? params.passcode.toLowerCase() : params.passcode;

	return { "passcode": passcode }
}
```


outputSchema
 ```json 
{
	"output": {
		"type": "object",
		"properties": {
			"passcode": {
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
| [gsw5wwtm7t](./gsw5wwtm7t.md) | [mt9kvt7hnn](./mt9kvt7hnn.md) |