# Automating the Login and MOTD Banner using Pythong

The `set_banner.py` Python script gets

1. the current configuration
2. the banner configuration
3. sets the login and motd banner
4. the banner configuration to verify the change

This Python code uses RESTCONF, which needs to be enabled on the device (usually disabled by default). To enable RESTCONF, run the following commands on the device:

```
IR1101(config)# restconf
IR1101(config)# ip http secure-server
```

This script can be used as-is with the [IR1101 DevNet Sandbox](https://devnetsandbox.cisco.com/DevNet/catalog/IR1101). If you are using your own device, change the IP address of the REST API urls.

**Note:** Remember to only use this script on a non-production environment.

## Resources

* [IR1101 DevNet Sandbox](https://devnetsandbox.cisco.com/DevNet/catalog/IR1101)
* [IR1101 Learning Lab](https://developer.cisco.com/learning/labs/iot-hardware-ir1101-sandbox/)