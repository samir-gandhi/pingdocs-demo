# Node - Password Authentication
## Configuration
ID:  rstodi2zw1

Type: CONNECTION 

CapabilityName: startNode

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




### Additional Properties
inputSchema
 ```json 
{
	"type": "object",
	"properties": {
		"email": {
			"type": "string",
			"displayName": "Email",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "email"
		},
		"password": {
			"type": "string",
			"displayName": "Password",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "password"
		},
		"rememberMe": {
			"type": "boolean",
			"displayName": "Remember Me",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "rememberMe"
		},
		"flowAccountRecoveryEnabled":{
			"type":"boolean",
            "displayName": "flowAccountRecoveryEnabled",
            "preferredControlType": "textField",
            "enableParameters": true,
            "propertyName": "flowAccountRecoveryEnabled"
		},		
		"flowMagicLinkEnabled":{
			"type":"boolean",
            "displayName": "flowMagicLinkEnabled",
            "preferredControlType": "textField",
            "enableParameters": true,
            "propertyName": "flowMagicLinkEnabled"
		},
		"flowPasswordlessRequired":{
			"type":"boolean",
            "displayName": "flowPasswordlessRequired",
            "preferredControlType": "textField",
            "enableParameters": true,
            "propertyName": "flowPasswordlessRequired"
		},
		"flowAgreementId": {
			"type":"string",
            "displayName": "flowAgreementId",
            "preferredControlType": "textField",
            "enableParameters": true,
            "propertyName": "flowAgreementId"
		},
		"flowAllowedDeviceTypes": {
			"type":"string",
            "displayName": "flowAllowedDeviceTypes",
            "preferredControlType": "textField",
            "enableParameters": true,
            "propertyName": "flowAllowedDeviceTypes"
		},
		"flowAgreementEnabled": {
			"type":"string",
            "displayName": "flowAgreementEnabled",
            "preferredControlType": "textField",
            "enableParameters": true,
            "propertyName": "flowAgreementEnabled"
		},
		"flowAppleEnabled":{
			"type":"boolean",
            "displayName": "flowAppleEnabled",
            "preferredControlType": "textField",
            "enableParameters": true,
            "propertyName": "flowAppleEnabled"
		},
		"flowFacebookEnabled":{
			"type":"boolean",
            "displayName": "flowFacebookEnabled",
            "preferredControlType": "textField",
            "enableParameters": true,
            "propertyName": "flowFacebookEnabled"
		},
		"flowGoogleEnabled":{
			"type":"boolean",
            "displayName": "flowGoogleEnabled",
            "preferredControlType": "textField",
            "enableParameters": true,
            "propertyName": "flowGoogleEnabled"
		},
        "flowMethod": {
			"type":"string",
            "displayName": "flowMethod",
            "preferredControlType": "textField",
            "enableParameters": true,
            "propertyName": "flowMethod"
        }
	}
}
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
|  | [bilu0ighwr](./bilu0ighwr.md) |