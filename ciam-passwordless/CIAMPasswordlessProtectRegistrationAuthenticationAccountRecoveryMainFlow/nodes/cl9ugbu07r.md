# Node - string 
Return Error
## Configuration
ID:  cl9ugbu07r

Type: CONNECTION 

CapabilityName: startNode

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | js 
Redirect back to requesting resource (error) | 





### Additional Properties
inputSchema
```json 
{
	"type": "object",
	"properties": {
		"errorMessage": {
			"type": "string",
			"displayName": "Error Message",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "errorMessage"
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




