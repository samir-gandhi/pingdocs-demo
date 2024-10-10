# Functions - Check If Device Removal Warning Is Needed
## Configuration
ID:  8sttri4np9

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
	const deviceRemovalWarning = params.size < 2
	return {&#39;deviceRemovalWarning&#39;: deviceRemovalWarning}
}
```


outputSchema
 ```json 
{
	"output": {
		"type": "object",
		"properties": {
			"deviceRemovalWarning": {
				"type": "boolean"
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
| [vbk955oxjg](./vbk955oxjg.md) | [4os42modvj](./4os42modvj.md) |