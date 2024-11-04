# Node - string 
PingOne Protect Analysis
## Configuration
ID:  h2wapsopzt

Type: CONNECTION 

CapabilityName: startNode

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | string 
This branch will perform a threat analysis using PingOne Protect feature. | 





### Additional Properties
inputSchema
```json 
{
	"type": "object",
	"properties": {
		"pingOneUserId": {
			"type": "string",
			"displayName": "User ID",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "pingOneUserId"
		},
		"SKRiskId": {
			"type": "string",
			"displayName": "SKRisk Id",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "SKRiskId"
		},
		"success": {
			"type": "boolean",
			"displayName": "success",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "success"
		}
	}
}
```




