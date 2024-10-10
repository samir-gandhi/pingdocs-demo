# Functions
## Configuration
ID:  psu8mrv4k9

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

	var returnAddress = {"streetAddress" : params.inputAddress, "postalCode": params.inputZipcode};

    var returnPhoto = {"href": params.inputPhoto}

	return {&#39;returnAddress&#39;: returnAddress, &#39;photo&#39; : returnPhoto}
}
```


outputSchema
 ```json 
{
	"output": {
		"type": "object",
		"properties": {
			"returnAddress": {
				"type": "object"
			},
			"photo": {
				"type": "object"
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
| [fxft0ouru8](./fxft0ouru8.md) | [9v2yv8gf4y](./9v2yv8gf4y.md) |