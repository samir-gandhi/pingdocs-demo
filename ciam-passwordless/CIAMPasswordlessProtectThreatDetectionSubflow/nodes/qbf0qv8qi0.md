# Functions - Flow Configuration Check
## Configuration
ID:  qbf0qv8qi0

Type: CONNECTION 

CapabilityName: customFunction

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Add input variables to check for null/empty | 
 




### Additional Properties
code
 ```json 
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


outputSchema
 ```json 
{
	"output": {
		"type": "object",
		"properties": {
			
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
|  | [6b03psy0ol](./6b03psy0ol.md) |