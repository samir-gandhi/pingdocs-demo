# Functions
## Configuration
ID:  psu8mrv4k9

Type: CONNECTION 

CapabilityName: customFunction





### Output Schema
``` json 
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

### Additional Properties
code
```js 
// Write your code here
// Supported language: Javascript 
module.exports = a = async ({params}) => {
	console.log(&#39;params: &#39;, params)

	var returnAddress = {"streetAddress" : params.inputAddress, "postalCode": params.inputZipcode};

    var returnPhoto = {"href": params.inputPhoto}

	return {&#39;returnAddress&#39;: returnAddress, &#39;photo&#39; : returnPhoto}
}
```


variableInputList
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [fxft0ouru8](./fxft0ouru8.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[9v2yv8gf4y](./9v2yv8gf4y.md) | 