# nodeWifiControlScanner


### Exxemplo 

```
var WiFiControl = require('wifi-control');
 
  //  Initialize wifi-control package with verbose output 
  WiFiControl.init({
    debug: true
  });
 
  //  Try scanning for access points: 
  WiFiControl.scanForWiFi( function(err, response) {
    if (err) console.log(err);
    console.log(response);
  });
  
  ```



### Exemplo Output:

```

{
    "success":  true,
    "networks":
      [ { "mac": "AA:BB:CC:DD:EE:FF",
          "channel": "1",
          "signal_level": "-43",
          "ssid": "Home 2.4Ghz" } ],
    "msg":"Nearby WiFi APs successfully scanned (1 found)."
  }
  
  ```
