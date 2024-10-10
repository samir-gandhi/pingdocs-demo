# Functions - Mask Phone Number/Email Address
## Configuration
ID:  o3p0lu1ww2

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
	let email = params.email
	let phone = params.phone

	if (email) {
		const [username, domain] = email.split("@");
  		const maskedUsername =
    	username.charAt(0) &#43; "*".repeat(username.length - 2) &#43; username.slice(-1);
		email = maskedUsername &#43; "@" &#43; domain;
	}

	if (phone) {
		// Strip all non-numeric characters from the phone number
  		const numericPhoneNumber = phone.replace(/\D/g, &#39;&#39;);
		// Mask the first six digits of the phone number
  		const maskedPhoneNumber = &#39;***-***-&#39; &#43; numericPhoneNumber.slice(-4);
		phone = maskedPhoneNumber;
	}
	return {&#39;maskedEmail&#39;: email, &#39;maskedPhone&#39;: phone}
}
```


outputSchema
 ```json 
{
	"output": {
		"type": "object",
		"properties": {
			"maskedEmail": {
				"type": "string"
			},
			"maskedPhone": {
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
| [522ujtnujz](./522ujtnujz.md) | [xceoebu0xh](./xceoebu0xh.md) |