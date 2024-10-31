# Functions - string 
Filter Unusable Devices
## Configuration
ID:  10uwd1ccc4

Type: CONNECTION 

CapabilityName: customFunction





### Output Schema
``` json 
{
  "output": {
    "type": "object",
    "properties": {
      "usableDevices": {
        "type": "array",
        "items": {
          "type": "string"
        }
      },
      "count": {
        "type": "number"
      },
      "canChangeDevice": {
        "type": "boolean"
      }
    }
  }
} 
```

### Additional Properties
code
```js 
module.exports = a = async ({ params }) => {
  var usableDevices = JSON.parse(params.devices);

  usableDevices = usableDevices.map(device => {
      if (device.type === "FIDO2" &amp;&amp; device?.attributes?.previousDeviceType) {
          return { ...device, type: device.attributes.previousDeviceType }
      }
      return device;
  });

  const allowedDeviceTypes = params.allowedDeviceTypes ? params.allowedDeviceTypes.split(",") : [];

  usableDevices = usableDevices.filter(device => {
      return allowedDeviceTypes.includes(device.type);
  });

  if (params.webAuthenSupport === "NONE") {
      usableDevices = usableDevices.filter(device => {
          return device.type !== "FIDO2";
      });
  }

  usableDevices = usableDevices.filter(device => {
      return device.coolDownExpiresAt == undefined;
  });
  
  let emailDevices = [];
  let smsDevices = [];
  let fido2Devices = [];
  
  for (let i = 0; i < usableDevices.length; i&#43;&#43;) {
    if (usableDevices[i].type === "EMAIL") {
      emailDevices.push(usableDevices[i]);
    } else if (usableDevices[i].type === "SMS") {
      smsDevices.push(usableDevices[i]);
    } else if (usableDevices[i].type === "FIDO2") {
      fido2Devices.push(usableDevices[i]);
    }
  }
  
  usableDevices = fido2Devices.concat(smsDevices, emailDevices);

  return { usableDevices: usableDevices, count: usableDevices.length, canChangeDevice: usableDevices.length > 1 || params.magicLinkEnabled}
}
```


variableInputList
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [9vk797lpxx](./9vk797lpxx.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[se271xaurx](./se271xaurx.md) | 