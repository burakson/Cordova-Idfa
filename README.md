### Identifier for Advertisers (IDFA) Plugin for PhoneGap/Cordova Applications

This cordova/phonegap plugin retrieves 'Identifier for Advertisers (IDFA)' from iOS > 6 devices.

More info [here](https://developer.apple.com/library/ios/documentation/AdSupport/Reference/ASIdentifierManager_Ref/ASIdentifierManager.html)

#### Supported Platforms

* iOS > 6.0

#### Installing 

Install with Cordova cli

    $ cordova plugin add https://github.com/burakson/Cordova-Idfa.git

Install with Phonegap cli

    $ phonegap plugin add https://github.com/burakson/Cordova-Idfa.git
    
#### Usage

* Add AdSupport.framework to the Linked Frameworks in Xcode

* After getting deviceReady event;

```javascript
Cordova.exec(cb, err, "CDVIdfa", "advertisingIdentifier", []);

function cb(m) {
  console.log('Device IDFA is '+m);
}

function err(m) {
  console.log('Error: '+m);
}
```

#### Feedback
    
Try the code. If you find a problem, file an issue or create a pull request.

#### Thanks
    
Thanks to [@choix](https://github.com/choix) a.k.a Anton Volkov
