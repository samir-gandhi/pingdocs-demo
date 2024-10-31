# Functions - string 
Filter Unusable Devices
## Configuration
ID:  pks46w5ks6

Type: CONNECTION 

CapabilityName: customFunction





### Output Schema
``` json 
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

### Additional Properties
code
```js 
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


variableInputList
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [4os42modvj](./4os42modvj.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[4wqs0nbs1v](./4wqs0nbs1v.md) | 