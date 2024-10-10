# Node - Authentication method selection
## Configuration
ID:  wc0jfkkr3z

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
		"usableDevices": {
			"type": "array",
			"displayName": "Usable Devices",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "usableDevices"
		},
		"rpid": {
			"type": "string",
			"displayName": "rpid",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "rpid"
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




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
|  | [k9rrvndxtf](./k9rrvndxtf.md) |