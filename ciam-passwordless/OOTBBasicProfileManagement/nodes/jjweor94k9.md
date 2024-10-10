# Functions - Extract Flow Parameters
## Configuration
ID:  jjweor94k9

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
	console.log(&#39;params: &#39;, params)

	return {&#39;username&#39;: params.flowParameters.username}
}
```


outputSchema
 ```json 
{
	"output": {
		"type": "object",
		"properties": {
			"username": {
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
|  | [bn2hi300ca](./bn2hi300ca.md) |