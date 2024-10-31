# Functions - string 
Get Device Info
## Configuration
ID:  5b5ckjqcix

Type: CONNECTION 

CapabilityName: customFunction





### Output Schema
``` json 
{
	"output": {
		"type": "object",
		"properties": {
			"type": {
				"type": "string"
			},
			"email": {
				"type": "string"
			},
			"phone": {
				"type": "string"
			},
			"displayName": {
				"type": "string"
			},
			"isDefault": {
				"type": "boolean"
			},
			"nickname": {
				"type": "string"
			},
			"applicationName": {
				"type": "string"
			},
			"marketingName": {
				"type": "string"
			}
		}
	}
} 
```

### Additional Properties
code
```js 
module.exports = a = async ({ params }) => {
	var devices = JSON.parse(params.devices);

	var selectedDevice = devices.filter(device => {
		return device.id == params.selectedDeviceId;
	});

	var isDefault = devices[0].id === params.selectedDeviceId;

	var nickname = selectedDevice[0].nickname;

	var applicationName = selectedDevice[0].application ? selectedDevice[0].application.nativeName : "";

	var marketingName = selectedDevice[0].model ? selectedDevice[0].model.marketingName : "";

	return {
		type: selectedDevice[0].type,
		email: selectedDevice[0].email,
		phone: selectedDevice[0].phone,
		displayName: selectedDevice[0].displayName,
		isDefault,
		nickname,
		applicationName,
		marketingName
	};
}
```


variableInputList
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [ako0e9ds26](./ako0e9ds26.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[088nn24g3r](./088nn24g3r.md) | 