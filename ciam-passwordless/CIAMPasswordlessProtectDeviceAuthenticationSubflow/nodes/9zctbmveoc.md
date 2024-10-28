# Functions - string 
Enrich Device Details
## Configuration
ID:  9zctbmveoc

Type: CONNECTION 

CapabilityName: customFunction





### Output Schema
``` json 
{
	"output": {
		"type": "object",
		"properties": {
			"selectedDeviceType": {
				"type": "string"
			},
			"selectedDeviceEmail": {
				"type": "string"
			},
			"selectedDevicePhone": {
				"type": "string"
			},
			"selectedDeviceName": {
				"type": "string"
			},
			"selectedDeviceOtpEnabled": {
				"type": "bool"
			}
		}
	}
} 
```

### Additional Properties
code
```js 
module.exports = a = async ({ params }) => {
	var selected = JSON.parse(params.devices).filter(device => {
		return device.id == params.id;
	});

	if (selected &amp;&amp; selected.length > 0 &amp;&amp; selected[0].hasOwnProperty("nickname")) {
  		var deviceName = selected[0].nickname;
	}

	if (selected[0].model) {
		deviceName = selected[0].model.marketingName;
	}

	if (selected[0].displayName) {
		deviceName = selected[0].displayName;
	}

	return {
		selectedDeviceType: selected[0].type,
		selectedDeviceEmail: selected[0].email,
		selectedDevicePhone: selected[0].phone,
		selectedDeviceName: deviceName,
		selectedDeviceOtpEnabled: selected[0].otpEnabled
	}
}
```


variableInputList
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [ybwxgols9w](./ybwxgols9w.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[1cbcpbc5no](./1cbcpbc5no.md) | 