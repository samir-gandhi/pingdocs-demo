# Node - string 
FIDO2
## Configuration
ID:  vc8o1wnpis

Type: CONNECTION 

CapabilityName: startNode






### Additional Properties
inputSchema
```json 
{
	"type": "object",
	"properties": {
		"authenticatorAttachment": {
			"type": "string",
			"displayName": "Authenticator Attachment",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "authenticatorAttachment"
		},
		"rpid": {
			"type": "string",
			"displayName": "rpid",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "rpid"
		},
		"type": {
			"type": "string",
			"displayName": "Type",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "type"
		},
		"usableDevices": {
			"type": "array",
			"displayName": "Usable Devices",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "usableDevices"
		},
		"origin": {
			"type": "string",
			"displayName": "origin",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "origin"
		}
	}
}
```




