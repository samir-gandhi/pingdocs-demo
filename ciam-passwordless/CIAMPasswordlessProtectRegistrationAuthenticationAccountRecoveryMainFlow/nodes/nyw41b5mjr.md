# Node - Check User
## Configuration
ID:  nyw41b5mjr

Type: CONNECTION 

CapabilityName: startNode

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Check if User is active | 
 




### Additional Properties
inputSchema
 ```json 
{
	"type": "object",
	"properties": {
		"useremail": {
			"type": "string",
			"displayName": "User Email",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "useremail"
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




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
|  | [iui85ujva3](./iui85ujva3.md) |