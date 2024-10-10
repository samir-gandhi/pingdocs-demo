# Functions - Set Flow Variables
## Configuration
ID:  umf4ie39n

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
	const results = {};

	const selectValue = (parameterValue, companyValue) => {
		if (params.flowParameters === undefined || parameterValue === undefined) {
			return companyValue;
		}

		return parameterValue === "true";
	};

	results["username"] = params.flowParameters.username;

	// allowed device types
	const isEmailOTPEnabled = selectValue(params.flowParameters.isEmailOTPEnabled, params.ciam_emailOtpEnabled);
	const isFidoPasskeyEnabled = selectValue(params.flowParameters.isFidoPasskeyEnabled, params.ciam_fidoPasskeyEnabled);
	const isSmsOTPEnabled = selectValue(params.flowParameters.isSmsOTPEnabled, params.ciam_smsOtpEnabled);	

	const devices = [];
	if (isEmailOTPEnabled) {
		devices.push("EMAIL");
	};
	if (isFidoPasskeyEnabled) {
		devices.push("FIDO2");
	};
	if (isSmsOTPEnabled) {
		devices.push("SMS");
	};

	results["flowAllowedDeviceTypes"] = devices.join(",");

	return { ...results };
}
```


outputSchema
 ```json 
{
	"output": {
		"type": "object",
		"properties": {
			"username": {
				"type": "boolean"
			},
			"flowAllowedDeviceTypes": {
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
|  | [efiecys0xw](./efiecys0xw.md) |