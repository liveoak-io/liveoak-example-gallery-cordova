Gallery Cordova Android Example
===============================

This demo application runs as a native application on a mobile device or emulator. It connects remotely to LiveOak endpoints provided by 'gallery' example application.


Installing the application
--------------------------

* Run Gallery application on LiveOak as described in Gallery Example README.md

* Open www/js/app.js, and set the value of HOST variable (line 2) to INET_ADDRESS where Gallery is running. Currently it is set to 10.0.2.2 which corresponds to a localhost running an Android emulator.

* Make sure to have latest version of cordova installed. This demo was tested with cordova@3.4.0-0.1.3
(NOTE: Updating cordova version might break applications using plugins from previous cordova versions. If you update your cordova version, make sure that you remove and reinstall all plugins again)

* Set up Cordova native Android project:

```shell
$ mkdir platforms plugins
$ cordova plugin add org.apache.cordova.inappbrowser
$ cordova plugin add org.apache.cordova.camera
$ cordova plugin add org.apache.cordova.file
$ cordova platform add android
````

Running the application
-----------------------

* Build native application from web app, and run it:

```shell
$ cordova run android
````

Whenever you change web application in www/ simply rerun the last command, to rebuild it as native Android app.

See detailed documentation [here](http://liveoak.io/docs/guides/tutorial_gallery/#gallery-for-android-using-cordova) .

