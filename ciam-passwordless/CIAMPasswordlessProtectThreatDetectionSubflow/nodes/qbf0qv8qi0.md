# Functions - string 
Flow Configuration Check
## Configuration
ID:  qbf0qv8qi0

Type: CONNECTION 

CapabilityName: customFunction

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
Add input variables to check for null/empty | 




### Output Schema
``` json 
{
	"output": {
		"type": "object",
		"properties": {
			
		}
	}
} 
```

### Additional Properties
code
```js 
// Iterate over params object, return false if any
// passed in parameters are null/empty
module.exports = a = async ({ params }) => {

	for (var key in params) {
		if (!params[key]) {
			return false; 
		}
	}

	return 
}
```


variableInputList
```
```




