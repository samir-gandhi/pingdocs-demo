# Functions - Create Masked Devices
## Configuration
ID:  wzzac3ucto

Type: CONNECTION 

CapabilityName: customFunction

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 




### Additional Properties
code
 ```json 
module.exports = a = async ({ params }) => {
  String.prototype.maskEmail = function() {
    const [username, domain] = this.split("@");
    const maskedUsername =
      username.charAt(0) &#43; "*".repeat(username.length - 2) &#43; username.slice(-1);
    return maskedUsername &#43; "@" &#43; domain;
  };

  String.prototype.maskPhoneNumber = function() {
    // Strip all non-numeric characters from the phone number
    const numericPhoneNumber = this.replace(/\D/g, &#39;&#39;);

    // Mask the first six digits of the phone number
    const maskedPhoneNumber = &#39;***-***-&#39; &#43; numericPhoneNumber.slice(-4);

    return maskedPhoneNumber;
  };

  var usableDevices = JSON.parse(params.devices);
  const magicLinkEmail = params.magicLinkEmail;

  for (let i = 0; i < usableDevices.length; i&#43;&#43;) {
    if (usableDevices[i].type === "EMAIL") {
      usableDevices[i].email = usableDevices[i].email.maskEmail();
    } else if (usableDevices[i].type === "SMS") {
      usableDevices[i].phone = usableDevices[i].phone.maskPhoneNumber();
    }
  }

  return { 
    maskedUsableDevices: usableDevices,
    maskedMagicLinkEmail: magicLinkEmail.maskEmail()
  }
}
```


outputSchema
 ```json 
{
  "output": {
    "type": "object",
    "properties": {
      "maskedUsableDevices": {
        "type": "array",
        "items": {
          "type": "string"
        }
      },
      "maskedMagicLinkEmail": {
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
| [se271xaurx](./se271xaurx.md) | [6yu5p2iz3r](./6yu5p2iz3r.md) |