<img src="build/icons/128x128.png" alt="logo" height="80" align="right" />

# (Electron) Outlook

The Outlook/Office365 desktop client.

![screenshot_linux](https://user-images.githubusercontent.com/13460738/35953459-a0875872-0ce9-11e8-9bca-880564b9beee.png)

## Feature
* Receive your hotmail / outlook online from the desktop app
* Close to minimise
* Dock tray support
* System notification

## Pre-Request
* [GIT](https://git-scm.com/)
* [YARN](https://yarnpkg.com/)

## Build & Install
Clone the repository and run in development mode.
```
git clone https://github.com/sier/outlook.git
cd electron-outlook
yarn
yarn start
```
Build the application 
```
yarn run dist:macos
```
This will build an App in the dist folder. This Mac applications works on macOS 10.10+

## Release
```
npm version (new release version)
git push origin master
git push origin --tags
npm publish
```

## Download
The released application can be downloaded [here](https://github.com/sier/outlook/releases).

## License
[MIT](https://github.com/eNkru/electron-xiami/blob/master/LICENSE) by [Howard J](https://enkru.github.io/)
