# Teleport - Create OTP Device
## Configuration
ID:  dc2mhwx86e

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
		"deviceType": {
			"type": "string",
			"displayName": "deviceType",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "deviceType"
		},
		"phone": {
			"type": "string",
			"displayName": "phone",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "phone"
		},
		"email": {
			"type": "string",
			"displayName": "email",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "email"
		},
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
		}
	}
}
```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
|  | [9a49qb1y7k](./9a49qb1y7k.md) |