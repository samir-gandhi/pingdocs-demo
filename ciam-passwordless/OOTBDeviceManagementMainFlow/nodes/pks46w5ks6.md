# Functions - Filter Unusable Devices
## Configuration
ID:  pks46w5ks6

Type: CONNECTION 

CapabilityName: customFunction

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




### Additional Properties
code
 ```json 
module.exports = a = async ({ params }) => {
  var usableDevices = JSON.parse(params.devices);

  const allowedDeviceTypes = params.allowedDeviceTypes ? params.allowedDeviceTypes.split(",") : [];

  usableDevices = usableDevices.filter(device => {
      return allowedDeviceTypes.includes(device.type);
  });

  usableDevices = JSON.stringify(usableDevices);

  return { usableDevices: usableDevices };
}
```


outputSchema
 ```json 
{
  "output": {
    "type": "object",
    "properties": {
      "usableDevices": {
        "type": "string"
      }
    }
  }
}
```


variableInputList
 ```json 

```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [4os42modvj](./4os42modvj.md) | [4wqs0nbs1v](./4wqs0nbs1v.md) |