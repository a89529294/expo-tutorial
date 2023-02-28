# Expo Tutorial

## Using Image Picker

- `npx expo install expo-image-picker`
- Reference `App.js` to see how it's used.

## Adding Gestures

- `npx expo install react-native-gesture-handler react-native-reanimated`
- `npm install -D @babel/plugin-proposal-export-namespace-from`
- Modify `babel.config.js` by adding `plugins: ["@babel/plugin-proposal-export-namespace-from","react-native-reanimated/plugin",],` to the returned object.
- because we modified `babel.config.js` we need to restart `npx expo start -c`. `-c` clears the cache.

## Taking and Saving Screenshots

- `npx expo install react-native-view-shot expo-media-library`
- `react-native-view-shot` allows taking a screenshot, `expo-media-library` allows accessing a device's media library to save an image.

## Splash Screen & App Icon

- Configure splash screen in `app.json` under the key `expo.splash`
- Configure how long splash screen stays by first `npx expo install expo-splash-screen` then adding the following to `app.js`

```js
import * as SplashScreen from "expo-splash-screen"

SplashScreen.preventAutoHideAsync()
setTimeout(SplashScreen.hideAsync, 5000)
```

- If you notice there is white bars around the splash screen modify the `expo.splash.backgroundColor` in `app.json` to match splash screen background.
-
