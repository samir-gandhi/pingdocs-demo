# Functions - Filter Unusable Device Types
## Configuration
ID:  kfqbhjjaqb

Type: CONNECTION 

CapabilityName: customFunction

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




### Additional Properties
code
 ```json 
module.exports = a = async ({ params }) => {
    console.log(&#39;params: &#39;, params)

    var usableDevices = JSON.parse(params.usableDevices);

    const allowedDeviceTypes = params.allowedDeviceTypes.split(",");
    const allowSMS = allowedDeviceTypes.some(device => device === "SMS");
    const allowEmail = allowedDeviceTypes.some(device => device === "EMAIL");
    const allowFIDO2 = allowedDeviceTypes.some(device => device === "FIDO2");
    
    if (params.webAuthenSupport === "NONE") {
        usableDevices = usableDevices.filter(device => {
            return device !== "SECURITY_KEY" &amp;&amp; device !== "PLATFORM" &amp;&amp; device !== "FIDO2";
        });
    }

    usableDevices = usableDevices.filter(device => {
        return (device === "SMS" &amp;&amp; allowSMS) 
            || (device === "EMAIL" &amp;&amp; allowEmail) 
            || (device === "FIDO2" &amp;&amp; allowFIDO2);
    })

    if (params.webAuthenSupport == "SECURITY_KEY_ONLY") {
        usableDevices = usableDevices.filter(device => {
            return device !== "PLATFORM";
        });
    }

    if (usableDevices.includes("SMS")) {
        const index = usableDevices.indexOf("SMS");
        if (index !== -1) {
            usableDevices.splice(index, 1);
            usableDevices.unshift("SMS");
        }
    }

    if (usableDevices.includes("FIDO2")) {
        const index = usableDevices.indexOf("FIDO2");
        if (index !== -1) {
            usableDevices.splice(index, 1);
            usableDevices.unshift("FIDO2");
        }
    }

    return { usableDevices: usableDevices, count: usableDevices.length }
}
```


outputSchema
 ```json 
{
  "output": {
    "type": "object",
    "properties": {
      "usableDevices": {
        "type": "array"
      },
      "count": {
        "type": "number"
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
| [tir7r8fvkp](./tir7r8fvkp.md) | [2ewaah2axe](./2ewaah2axe.md) |