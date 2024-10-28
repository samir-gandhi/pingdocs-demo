# Node - string 
Return Success
## Configuration
ID:  x8uq3h1ccd

Type: CONNECTION 

CapabilityName: startNode

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | js 
Redirect back to requesting resource (success) | 





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
		"authenticationMethods": {
			"type": "string",
			"displayName": "Any authentication method used separated by space.",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "authenticationMethods"
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




