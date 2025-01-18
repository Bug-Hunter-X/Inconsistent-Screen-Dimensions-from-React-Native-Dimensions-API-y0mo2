# Inconsistent Screen Dimensions in React Native

This repository demonstrates a bug related to inconsistent screen dimension values returned by the `Dimensions` API in React Native. The issue is characterized by occasional inaccuracies in the reported width and height, leading to layout inconsistencies across different devices and screen orientations. 

## Problem

The `Dimensions` API, while generally reliable, may sometimes provide incorrect or inconsistent dimension values. This isn't a consistent crash, but rather subtle inaccuracies that manifest in unpredictable ways, making debugging difficult. This can lead to layouts that break unpredictably and are hard to fix. 

## Solution

The provided solution explores a workaround involving a slight delay or using `Dimensions.addEventListener` to listen for changes. Although it isn't a perfect fix for all scenarios, it can improve consistency, especially in components that are sensitive to dimension changes.

## How to Reproduce

1. Clone this repository.
2. Navigate to the project directory using your terminal.
3. Run `npm install` to install dependencies.
4. Run `npx react-native run-android` or `npx react-native run-ios` to run the app on an emulator or device.
5. Observe the layout. Rotate the device or change the emulator screen size to see the inconsistency.

## License

MIT