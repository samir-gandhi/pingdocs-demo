# Functions - Update error message
## Configuration
ID:  5vhs0j1lcd

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
	let result = "";
	// Parse the password policy requirements in the detailed error message and pass it back to the form to map the proper errors.
	if (params.errorDetails &amp;&amp;
  		params.errorDetails.details &amp;&amp;
  		params.errorDetails.details[0] &amp;&amp;
  		params.errorDetails.details[0].rawResponse &amp;&amp;
  		params.errorDetails.details[0].rawResponse.details &amp;&amp;
  		params.errorDetails.details[0].rawResponse.details[0].innerError) {
		const details = params.errorDetails.details[0].rawResponse.details[0].innerError;
		result = "passwordPolicies:";
		for (let key in details) {
			if (details.hasOwnProperty(key) &amp;&amp; key !== "unsatisfiedRequirements") {
				switch (key) {
					case "minCharacters":
						const reason = details[key];

						if (reason.includes("ZYXWVUTSRQPONMLKJIHGFEDCBA")) {
							result &#43;= " minCharactersUppercase";
						}
						if (reason.includes("~!@#$%^&amp;*()-_=&#43;[]{}|;:,.<>/?")) {
							result &#43;= " minCharactersSpecialChar";
						}
						if (reason.includes("0123456789")) {
							result &#43;= " minCharactersNumeric";
						}
						if (reason.includes("abcdefghijklmnopqrstuvwxyz")) {
							result &#43;= " minCharactersLowercase";
						}
						break;
					case "minUniqueCharacters":
						result &#43;= " minUniqueCharacters";
						break;
					case "excludesCommonlyUsed":
						result &#43;= " excludesCommonlyUsed"
						break;
					case "length":
					// Parse the length requirement
						const value = details[key];
						const index = value.indexOf("of");
						if (index !== -1 &amp;&amp; index < value.length - 1) {
							let lengthRestriction = value[index &#43; 3];
							if (value[index &#43; 4] !== " ") {
								lengthRestriction = lengthRestriction &#43; value[index &#43; 4];
							}
							result &#43;= " length" &#43; lengthRestriction;
						}
						break;
					case "maxRepeatedCharacters":
						result &#43;= " maxRepeatedCharacters";	
						break;	
					default:
						result &#43;= details[key];					

				}
			}
		}
	} else {
		let errorMessage = params.errorDetails.details[0].rawResponse.details[0].innerError.history;
		let index = errorMessage.indexOf(&#39;:&#39;);
		if (index !== -1) result = errorMessage.substring(index &#43; 2);
		else result = errorMessage;
	}

	return {&#39;updatedErrorMessage&#39;: result.replace(&#39;username&#39;, &#39;email address&#39;)}
}
```


outputSchema
 ```json 
{
	"output": {
		"type": "object",
		"properties": {
			"updatedErrorMessage": {
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
| [uh6ap9pj4p](./uh6ap9pj4p.md) | [kj7e51zikv](./kj7e51zikv.md) |