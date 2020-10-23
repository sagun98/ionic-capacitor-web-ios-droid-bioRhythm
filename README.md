# Biorhythm Calculator

## Links

 * [Biorhythm](https://en.wikipedia.org/wiki/Biorhythm) Wikipedia entry
 * [Biorhythm Calculator](https://keisan.casio.com/exec/system/1340246447) by Casio


## Capacitor documentation 
- npm install @capacitor/core --save-exact
- npm install @capacitor/cli --save-exact
- npx cap init --web-dir build --npm-client npm Biorhythms com.tngin.bio

## Android
- npx cap add android  (Pin dependency removing cap in package.json)
- npx cap open android
- npx cap sync android


For Live Reload in Android Studio emulator, add following in capacitor.config.json 
"server":{
    "url":"http://10.0.0.11:3000"
}

## IOS
- npx cap add ios
- npx cap open ios
- npx cap sync ios

## Fix the header thingy in IOS app 
- Add following in /public/index.html      
```<meta name="viewport" content="viewport-fit=cover, width=device-width, initial-scale=1" />```

## Resource generator
- npm i -g cordova-res
- npx cordova-res android --skip-config --copy --unsafe-perm
- npx cordova-res ios --skip-config --copy


## IONIC CLI
- npm install -g @ionic/cli
- ionic start ionic-cli-app blank --type=react --capacitor