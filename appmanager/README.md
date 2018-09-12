## Elastos appmanager plugin

###  Preconditions
- The user creates an ionic project and copies the appmanager directory to the project directory
- Currently appmanager only supports android platform

### Installing the plugin
ionic cordova plugin add appmanager

### Using plugins
1. Add in front of the ts file
```
"Declare let cordova: any;
```
2. Call the start method of appmannager
```
cordova.plugins.appmanager.StartApp(url + "?timestamp=" + new Date() .getTime(), function (data) { }, function (error) { });
```