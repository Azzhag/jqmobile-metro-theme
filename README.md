# Welcome #

Project aim is to build Metro UI HTML5-based theme on top of jQuery Mobile to mimic Windows Phone 7 native look and feel.

# Components #

### Metro theme ##

Metro theme is presented by jquery.mobile.metro.theme.css file and related images folder.

    /themes/metro/

### Additional plugins ###

All additional theme plugins are located at /plugins folder

    /plugins/app-bar/ - Windows Phone alike ApplicationBar control

    /plugins/date-picker/ - Date and Time picker. Note: if runs under Cordova environment and there is Cordova DateTimePicker
    plugin then it uses native UI instead of html

    /plugins/progress-bar/ - implements porgress bar control

    /plugins/toggle-button/ - toggle button

** Each plugin folder contains sample page with usage example.

There is also special js code exporting theme switching functionality located at

    /themes/themeswitcher/jquery.mobile.themeswitcher.js

### Cordova ###

The theme provides additional level of functionality when viewing on the phone under Cordova framework. This is implemented
by the following cordova plugins.

backButtonHandler.js - hardware back button handling functionality

dateTimePicker.js - js bridge for Cordova native DateTimePicker

jquery.cordova.metro.themeswitcher.js - provides functionality to apply system colors (uses phoneTheme.js below)

phoneTheme.js - js bridge for Cordova system colors detection plugin

### Samples ###

Demo pages for the jquerymobile.com site reference (official demo for other developers).

    /samples/jqm-public-demo/index.html

Windows Phone application based on Cordova framework to demonstrate all theme functionality (system colors, native UI elements).
Does not contain any html pages inside, it uses absolute reference to test pages (see next section) located remotly.

    /samples/WindowsPhone/MetroThemeDemoApp

### Test pages ###

jQuery Mobile gallery sample page (with some little modifications). Contains both html version and windows phone native application.

    /tests/basic/gallery/

This sample page demonstrates all metro theme additional plugins/controls descibed above ('Additional plugins' section). Html only verison.

    /tests/extra/all.html

Note. Pages above are used as a reference for Windows Phone demo application.

## Prerequisite (Windows Phone only) ##
(No actions are required to run html samples and test pages.)

Silverlight for Windows Phone Toolkit is required to build
http://silverlight.codeplex.com/releases/view/71550#DownloadId=270984

# Usage #

### To run jqmobile demo ###
1. Deploy to server the following directory (optional, you can run the demo from file system)
    /samples/jqm-public-demo/
2. Navigate to (desktop or mobile browser)
    jqm-public-demo/index.html

### To run gallery test pages ###
1. Deploy to server the following directories (optional, you can run the demo from file system)
   /cordova
   /jqmobile-core
   /plugins
   /tests
   /themes
2. Navigate to (desktop or mobile browser)
    /tests/basic/gallery/html/forms-all.html

### To build Windows Phone demo app ###
1. Open the following solution in Visual Studio
    /samples/WindowsPhone/MetroThemeDemoApp/MetroThemeDemoApp.sln
2. Update CordovaView.StartPageUri (MainPage.xaml) to reference to /tests/basic/gallery/html/forms-all.html located remotly.
3. Build

## Links ##

Theme whe web version (doesn’t fully reflect the device experience)

http://mshare.akvelon.net:8184/metro/tests/basic/gallery/html/forms-all.html

Web demo for the jquerymobile.com site reference

http://mshare.akvelon.net:8184/metro/samples/jqm-public-demo/index.html

Windows Phone demo app (restricted access)

http://windowsphone.com/s?appid=f62a1b8b-b4db-4066-b825-1139e5b9f57a



