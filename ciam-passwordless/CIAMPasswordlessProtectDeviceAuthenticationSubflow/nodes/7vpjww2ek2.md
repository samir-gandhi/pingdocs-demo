# Node - FIDO2
## Configuration
ID:  7vpjww2ek2

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
		"success": {
			"type": "boolean",
			"displayName": "success",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "success"
		},
		"type": {
			"type": "string",
			"displayName": "Type",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "type"
		},
		"publicKeyCredentialCreationOptions": {
			"type": "string",
			"displayName": "publicKeyCredentialCreationOptions",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "publicKeyCredentialCreationOptions"
		},
		"canChangeDevice": {
			"type": "boolean",
			"displayName": "canChangeDevice",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "canChangeDevice"
		},
		"usableDevices": {
			"type": "object",
			"displayName": "Usable Devices",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "usableDevices"
		},
		"maskedUsableDevices": {
			"type": "object",
			"displayName": "Masked Usable Devices",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "maskedUsableDevices"
		},
		"deviceAuthId": {
			"type": "string",
			"displayName": "Device Authentication ID",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "deviceAuthId"
		},
		"origin": {
			"type": "string",
			"displayName": "origin",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "origin"
		},
		"pingOneUserId": {
			"type": "string",
			"displayName": "PingOne User ID",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "pingOneUserId"
		},
		"maskedMagicLinkEmail": {
			"type": "string",
			"displayName": "Masked Magic Link Email",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "maskedMagicLinkEmail"
		}	
	}
}
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
|  | [t04dles3gs](./t04dles3gs.md) |