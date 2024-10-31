# Functions - string 
Extract Flow Parameters
## Configuration
ID:  jjweor94k9

Type: CONNECTION 

CapabilityName: customFunction





### Output Schema
``` json 
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

### Additional Properties
code
```js 
// Write your code here
// Supported language: Javascript 
module.exports = a = async ({params}) => {
	console.log(&#39;params: &#39;, params)

	return {&#39;username&#39;: params.flowParameters.username}
}
```


variableInputList
```
```




