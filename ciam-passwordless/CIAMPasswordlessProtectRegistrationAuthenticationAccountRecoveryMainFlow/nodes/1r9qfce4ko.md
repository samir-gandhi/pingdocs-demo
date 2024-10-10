# Node - Authentication Complete
## Configuration
ID:  1r9qfce4ko

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
		"rememberMe": {
			"type": "boolean",
			"displayName": "Remember Me",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "rememberMe"
		},
		"pingOneUserId": {
			"type": "string",
			"displayName": "User ID",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "pingOneUserId"
		},
		"authenticationMethods": {
			"type": "string",
			"displayName": "Any authentication method used separated by space.",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "authenticationMethods"
		},
		"lifeCycleStatus": {
			"type": "string",
			"displayName": "Life Cycle Status",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "lifeCycleStatus"
		},
		"flowAgreementId": {
			"type":"string",
            "displayName": "flowAgreementId",
            "preferredControlType": "textField",
            "enableParameters": true,
            "propertyName": "flowAgreementId"
		},
		"flowAgreementEnabled": {
			"type":"boolean",
            "displayName": "flowAgreementEnabled",
            "preferredControlType": "textField",
            "enableParameters": true,
            "propertyName": "flowAgreementEnabled"
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
|  | [n2c0bh5gsg](./n2c0bh5gsg.md) |