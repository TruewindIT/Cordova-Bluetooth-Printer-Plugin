# Cordova-Bluetooth-Printer-Plugin
A cordova plugin for bluetooth printer for android platform.

##Support
- Text
- POS
- ZPL and ZPL Commands

##Install
Using the Cordova CLI and NPM, run:

```
cordova plugin add https://github.com/TruewindIT/Cordova-Bluetooth-Printer-Plugin
```


##Usage
Get list of paired bluetooth printers

```
BTPrinter.list(function(data){
        console.log("Success");
        console.log(data); \\list of printer in data array
    },function(err){
        console.log("Error");
        console.log(err);
    })
```


Connect printer

```
BTPrinter.connect(function(data){
	console.log("Success");
	console.log(data)
},function(err){
	console.log("Error");
	console.log(err)
}, "PrinterName")
```


Disconnect printer

```
BTPrinter.disconnect(function(data){
	console.log("Success");
	console.log(data)
},function(err){
	console.log("Error");
	console.log(err)
}, "PrinterName")
```


Disconnect printer

```
BTPrinter.disconnect(function(data){
	console.log("Success");
	console.log(data)
},function(err){
	console.log("Error");
	console.log(err)
})
```


Print simple string

```
BTPrinter.printText(function(data){
    console.log("Success");
    console.log(data)
},function(err){
    console.log("Error");
    console.log(err)
}, "String to Print")
```

POS printing

```
BTPrinter.printPOSCommand(function(data){
    console.log("Success");
    console.log(data)
},function(err){
    console.log("Error");
    console.log(err)
}, "0C")
//OC is a POS command for page feed
```