# Functions - string 
Set Industry Variables
## Configuration
ID:  4rjs3llu20

Type: CONNECTION 

CapabilityName: customFunction





### Output Schema
``` json 
{
	"output": {
		"type": "object",
		"properties": {
			"flowCompanyLogo": {
				"type": "string"
			},
			"flowCompanyGreeting": {
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
	const { 
		ciam_logoUrl, 
		ciam_companyName, 
		ciam_logoStyle,
		flowMethod
	} = params;

	const flowCompanyLogo = (flowMethod === &#39;WIDGET&#39;) 
		? `<div class="dialog-content-header dialog-content__header" style="height: 85px"><div class="dialog-content-header__logo"></div></div>`
		: `<img class="align-self-center mb-5" src="${ciam_logoUrl}" alt="${ciam_companyName}" style="${ciam_logoStyle}"></img>`;

	const flowCompanyGreeting = (flowMethod === &#39;WIDGET&#39; )
		? &#39;<p class="text-muted text-center mb-5"></p>&#39;
		: `<p class="text-muted text-center">Welcome to ${ciam_companyName}</p>`;

	return { flowCompanyLogo, flowCompanyGreeting }
}
```


variableInputList
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [2t8o7qakxh](./2t8o7qakxh.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[340awenest](./340awenest.md) | 