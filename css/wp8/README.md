# Welcome #

This theme provides a Windows Phone user interface for <a href="http://http://incubator.apache.org/cordova/">Apache Cordova</a> apps using jQuery Mobile on Windows Phone 8.

### Live demo ###

Web demo

http://sgrebnov.github.com/jqmobile-wp8-theme/samples/jqm-public-demo/index.html

Windows Phone 8 demo app

http://windowsphone.com/s?appid=tbd

### Copyrights ###
    Licensed under the Apache License, Version 2.0 (the "License");
	you may not use this file except in compliance with the License.
	You may obtain a copy of the License at

	http://www.apache.org/licenses/LICENSE-2.0

	Unless required by applicable law or agreed to in writing, software
	distributed under the License is distributed on an "AS IS" BASIS,
	WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
	See the License for the specific language governing permissions and
	limitations under the License.

# Components #

### jQM theme for Windows Phone ##

jQM theme for Windows Phone is presented by jquery.mobile.wp.theme.css file and related images folder.

    /themes/wp/

### Additional plugins ###

All additional theme plugins are located at /plugins folder

    /plugins/app-bar/ - an Application Bar

    /plugins/date-picker/ - Apache Cordova plugin for WP that exposes the native DateTime picker

    /plugins/progress-bar/ - implements porgress bar control

    /plugins/toggle-button/ - toggle button

** Each plugin folder contains sample page with usage example.

There is also special js code exporting theme switching functionality located at

    /themes/themeswitcher/jquery.mobile.themeswitcher.js

### Apache Cordova ###

The jQM theme for Windows Phone is designed to work with Apache Cordova on Windows Phone 7.5 for optimal integration. This is implemented
by the following Apache Cordova plugins.

backButtonHandler.js - hardware back button handling functionality

dateTimePicker.js - js bridge for Apache Cordova native DateTimePicker

jquery.cordova.wp.themeswitcher.js - provides functionality to apply system colors (uses phoneTheme.js below)

phoneTheme.js - js bridge for Apache Cordova system colors detection plugin

### Samples ###

Official demo for other developers.

    /samples/jqm-public-demo/index.html

Windows Phone application based on Apache Cordova framework to demonstrate all theme functionality (system colors, native UI elements).
Does not contain any html pages inside, it uses absolute reference to test pages (see next section) located remotly.

    /samples/WindowsPhone8/jQMThemeForWindowsPhone

### Test pages ###

jQuery Mobile gallery sample page (with some little modifications). Contains both html version and windows phone native application.

    /tests/basic/gallery/

This sample page demonstrates all jQM theme for Windows Phone additional plugins/controls descibed above ('Additional plugins' section). Html only verison.

    /tests/extra/all.html

Note. Pages above are used as a reference for Windows Phone demo application.

## Prerequisite ##
The following componets are required for optimal theme work
Apache Cordova App on Windows Phone 8
Silverlight for Windows Phone Toolkit
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
1. Open the following solution in Visual Studio 2012 or above
    /samples/WindowsPhone8/jQMThemeForWindowsPhone/jQMThemeForWindowsPhone.sln
2. Update CordovaView.StartPageUri (MainPage.xaml) to reference to /tests/basic/gallery/html/forms-all.html located remotly.
3. Build

# Nuget packages for Visual Studio #

<a href="https://www.nuget.org/packages/jQMThemeForWindowsPhone8">jQMThemeForWindowsPhone8</a>

This nuget package allows developers to apply a Windows Phone style look and feel to Windows Phone HTML5 applications developed with Apache Cordova and jQuery Mobile on Windows Phone 8.

To install jQMThemeForWindowsPhone8, run the following command in the Package Manager Console

    Install-Package jQMThemeForWindowsPhone8

<a href="https://www.nuget.org/packages/jQMThemeForWindowsPhone8Lite">jQMThemeForWindowsPhone8Lite</a>

This nuget package allows developers to apply a Windows Phone style look and feel to applications developed with 'Windows Phone HTML5 App' Visual Studio project template and jQuery Mobile on Windows Phone 8.

To install jQMThemeForWindowsPhone8Lite, run the following command in the Package Manager Console

    Install-Package jQMThemeForWindowsPhone8Lite