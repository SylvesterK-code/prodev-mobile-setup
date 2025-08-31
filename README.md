# prodev-mobile-setup
Mobile Development with React Native


# prodev-mobile-setup
Mobile Development with React Native

# Mobile Development Setup

## Tools Installed
- Node.js v18.x
- VS Code
- Expo Go (Android/iOS)
- Expo CLI (new version via npx)

## Setup Steps
1. Installed Node.js LTS.
2. Installed Expo Go on my phone from the [Expo Go](https://expo.dev/go) page.
3. Uninstalled old `expo-cli` and switched to the new local CLI.
4. Created a sample app using `npx create-expo-app`.
5. Tested app successfully on physical device using Expo Go.

## Challenges Faced
- Saw warning about legacy `expo-cli` not supporting Node.js 17+.
- Fixed it by migrating to the new CLI.






.
--------------------------------------------------------------------------------------------------------------





# Mobile Development Environment Setup

## Objective
Set up and test the mobile development environment using Expo Go, Node.js, and VS Code.

## Tools Installed
- **Node.js LTS**: v18.x
- **npm**: v9.x
- **VS Code**
- **Expo CLI** (optional)
- **Expo Go App** on Android/iOS

## Setup Process
1. Installed Node.js LTS from https://nodejs.org/
2. Verified Node.js and npm installation.
3. Installed VS Code and React Native extensions.
4. Installed Expo CLI globally.
5. Installed Expo Go app on my device and signed in.
6. Created a test project using `npx create-expo-app my-first-app`.
7. Ran `npx expo start` and successfully opened the app via QR code.

## Challenges Faced
- [Document any challenges you encountered, like network issues, installation errors, etc.]

## Next Steps
- Start building React Native mini-projects using Expo.



Task 1 1. Create Your First Mobile App
---------------------------------------------------------------------------------------------------------------
Steps you followed for scaffolding your Expo project

Observations from running the npx expo reset-project command

# Expo Project Setup

## 1. Steps for Scaffolding the Project
1. **Installed Node.js (LTS version)**  
   - Verified installation with:  
     ```bash
     node -v
     npm -v
     ```

2. **Installed Expo CLI locally using NPX**  
   ```bash
   npx create-expo-app prodev-mobile-setup


Navigated into the project folder

cd prodev-mobile-setup


Started the development server

npx expo start


Opened the app in Expo Go on a physical device or emulator.

2. Observations from npx expo reset-project

The reset-project command performs a cleanup and reset of the Expo project:

npx expo reset-project


Key Observations:

moves the app to app-example instead of deleting it.

Cleans up existing configurations and resets cache.

Removes and reinitializes node_modules, package-lock.json, and .expo cache folders.

Regenerates project settings (Metro bundler cache, Expo cache, etc.).

Ensures a clean and consistent development environment.

This command is useful if:

You encounter unexpected build errors.

You change major dependencies and want a fresh start.

You want to ensure your local environment matches the package.json definitions.

3. Notes

Recommended Node.js version: 20.x LTS

Recommended Expo CLI version: 0.24.x


3. Fixing React Native Version Mismatch

During setup, Expo showed:

react-native@0.79.6 - expected version: 0.79.5


To fix this:

Check the expected version:

npx expo install react-native


This installs the exact version Expo expects.

Reinstall dependencies:

rm -rf node_modules package-lock.json
npm install


Verify installation:

npx expo doctor


Should confirm all dependencies are aligned.

Restart the project:

npx expo start

4. Notes

Recommended Node.js version: 20.x LTS

Recommended Expo CLI version: 0.24.x

Always use npx expo install <package> to ensure correct versions for Expo SDK.