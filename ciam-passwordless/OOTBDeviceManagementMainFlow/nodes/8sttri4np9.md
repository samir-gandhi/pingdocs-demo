# Functions - string 
Check If Device Removal Warning Is Needed
## Configuration
ID:  8sttri4np9

Type: CONNECTION 

CapabilityName: customFunction





### Output Schema
``` json 
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

### Additional Properties
code
```js 
// Write your code here
// Supported language: Javascript 
module.exports = a = async ({params}) => {
	const deviceRemovalWarning = params.size < 2
	return {&#39;deviceRemovalWarning&#39;: deviceRemovalWarning}
}
```


variableInputList
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [vbk955oxjg](./vbk955oxjg.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[4os42modvj](./4os42modvj.md) | 