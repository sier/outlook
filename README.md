# Outlook Web Application as a dedicated application [![Build Status](https://travis-ci.com/sier/outlook.svg?branch=master)](https://travis-ci.com/sier/outlook)
This provides installers for Windows/Mac/Linux that install a dedicated application which hosts outlook's web application. 

![Image of Application](https://i.imgur.com/DrZQZwOh.jpg)

# Rationale
I have found that the Outlook Web application a great email client for a number of reasons.
* It always is running the latest without upgrading.
* It gets new features faster (such as sweep)
* It starts fast and is really responsive.
* etc

The one thing that has prevented me from adopting it is the fact that it runs as a browser tab. 
* It gets lost in the soup of other tabs
* It is harder to get to my email tab because it isn't on my active app list
* Browser hot keys sometimes interact with the application 
* It doesn't give me notifications when the brower goes away
etc.

To solve this I have created (well forked eNkrus version and tweaked) an Electron app which simply runs the Outlook Web app in a dedicated application frame:

## Outlook 365 application
This hosts http://mail.office365.com and is suitable for using with enterprise work/school environments

## Outlook.com application
This hosts http://outlook.com and is suitable for using for personal email.

# Installing
Go to https://github.com/sier/outlook/releases
* **.app** version installs on mac

# Building
Install prerequistites
```bash
yarn
```

## Building Outlook.com version
Go to Outlook.com folder and run 
```bash
yarn run dist:win
yarn run dist:macos
yarn run dist:linux
``` 
To build each distribution for outlook.com.  The installers will be built into the dist folder.


## Building Office 365 version
Go to Office365  folder and run 
```bash
yarn run dist:win
yarn run dist:macos
yarn run dist:linux
``` 
To build each distribution for office365.  The installers will be built into the dist folder.

# Acknowledgements
This project is a fork of:

* [eNkru/freelook](https://github.com/eNkru/freelook)
  * [tomlm/electron-outlook](https://github.com/tomlm/electron-outlook)
