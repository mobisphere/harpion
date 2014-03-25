harpion - harpjs + ionic-angular-cordova-seed
=============================================

The starting point for an Ionic project with Harp.


### Setup

Install required tools

```bash
$ npm install -g cordova ionic harp ripple-emulator
```


### Development and Testing

Access development environment at http://localhost:9000 (Port 9000 is default; change port using `--port` or `-p` option)

```bash
$ harp server app
```


__Test using Ripple emulator:__

```bash 
ripple emulate --path http://localhost:9000
```
and open browser at ```http://localhost:9000/?enableripple=cordova-2.0.0```

__Test using an Android emulator:__

```bash
$ harp compile app www
$ cordova platform add android
$ ionic emulate android
```


### Production

Generate static assets in ```www``` folder and run on Android device

```bash
$ harp compile app www
$ ionic run android
```


### Credits:
- [Harpjs](http://harpjs.com/)
- [Ionic](http://ionicframework.com/)
