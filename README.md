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
