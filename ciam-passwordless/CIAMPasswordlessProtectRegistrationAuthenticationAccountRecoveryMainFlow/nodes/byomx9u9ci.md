# Functions - Set Flow Variables
## Configuration
ID:  byomx9u9ci

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
	const results = { flowMethod: "REDIRECT" };

	const selectValue = (parameterValue, companyValue) => {
		if (params.flowParameters === undefined || parameterValue === undefined) {
			return companyValue;
		}

		// Assume WIDGET if any flowParameters is found
		results.flowMethod = "WIDGET";

		return parameterValue === "true";
	};

	// flow path variables
	results["flowAccountRecoveryEnabled"] = selectValue(params.flowParameters.isAccountRecoveryEnabled, params.ciam_accountRecoveryEnabled);
	results["flowMagicLinkEnabled"] = selectValue(params.flowParameters.isEmailMagicLinkEnabled, params.ciam_magicLinkEnabled);
	results["flowAgreementEnabled"] = selectValue(params.flowParameters.isTermsOfServiceEnabled, params.ciam_agreementEnabled);
	results["flowPasswordlessRequired"] = selectValue(params.flowParameters.isPasswordlessRequired, params.ciam_passwordlessRequired);

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

	// social logins
	results["flowAppleEnabled"] = selectValue(params.flowParameters.isAppleEnabled, params.ciam_appleEnabled);
	results["flowFacebookEnabled"] = selectValue(params.flowParameters.isFacebookEnabled, params.ciam_facebookEnabled);
	results["flowGoogleEnabled"] = selectValue(params.flowParameters.isGoogleEnabled, params.ciam_googleEnabled);

	results["flowSocialRegistrationEnabled"] = results["flowAppleEnabled"] || results["flowFacebookEnabled"] || results["flowGoogleEnabled"];

	return { ...results };
}
```


outputSchema
 ```json 
{
	"output": {
		"type": "object",
		"properties": {
			"flowAccountRecoveryEnabled": {
				"type": "boolean"
			},
			"flowMagicLinkEnabled": {
				"type": "boolean"
			},
			"flowAgreementEnabled": {
				"type": "boolean"
			},
			"flowPasswordlessRequired": {
				"type": "boolean"
			},
			"flowAllowedDeviceTypes": {
				"type": "string"
			},
			"flowAppleEnabled": {
				"type": "boolean"
			},
			"flowFacebookEnabled": {
				"type": "boolean"
			},
			"flowGoogleEnabled": {
				"type": "boolean"
			},
			"flowSocialRegistrationEnabled": {
				"type": "boolean"
			},
			"flowMethod": {
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
| [3lgnmx50te](./3lgnmx50te.md) | [2t8o7qakxh](./2t8o7qakxh.md) |