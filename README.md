# NavigationApp - Lab 8

**Student:** Adam Walters  
**Student ID:** N01701019  
**Course:** CPAN 213 - Cross-Platform Mobile Application Development  
**Date:** November 15, 2025

## Project Overview

Multi-screen navigation app demonstrating React Navigation with Stack and Tab navigators.

## Features Implemented

- ✅ Stack Navigator with 3 screens (Home, Details, Profile)
- ✅ Tab Navigator with 3 tabs (Home, Search, Settings)
- ✅ Parameter passing between screens
- ✅ Custom header styling
- ✅ Navigation actions (navigate, goBack, setParams)

## Installation

```bash
# Clone repository
git clone https://github.com/Sancoltos/NavigationApp
cd NavigationApp

# Install dependencies
npm install

# iOS setup
cd ios && pod install && cd ..

# Run on iOS
npx react-native run-ios

# Run on Android
npx react-native run-android
```

## Project Structure

```
NavigationApp/
├── src/
│   ├── navigation/
│   │   ├── StackNavigator.js
│   │   └── TabNavigator.js
│   └── screens/
│       ├── HomeScreen.js
│       ├── DetailsScreen.js
│       ├── ProfileScreen.js
│       ├── SearchScreen.js
│       └── SettingsScreen.js
├── App.js
└── index.js
```

## Navigation Flow

- **Tab 1 (Home):** Stack Navigator containing Home → Details → Profile screens
- **Tab 2 (Search):** Search screen with text input
- **Tab 3 (Settings):** Settings screen with toggle switches

## Testing

All navigation features have been tested:
- Stack navigation with parameter passing
- Tab switching functionality
- Back button navigation
- Dynamic header updates
- Parameter updates with setParams()

## Dependencies

- @react-navigation/native
- @react-navigation/stack
- @react-navigation/bottom-tabs
- react-native-screens
- react-native-safe-area-context
- react-native-gesture-handler
- react-native-vector-icons
