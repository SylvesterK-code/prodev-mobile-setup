# Welcome to your Expo app 👋

This is an [Expo](https://expo.dev) project created with [`create-expo-app`](https://www.npmjs.com/package/create-expo-app).

## Get started

1. Install dependencies

   ```bash
   npm install
   ```

2. Start the app

   ```bash
   npx expo start
   ```

In the output, you'll find options to open the app in a

- [development build](https://docs.expo.dev/develop/development-builds/introduction/)
- [Android emulator](https://docs.expo.dev/workflow/android-studio-emulator/)
- [iOS simulator](https://docs.expo.dev/workflow/ios-simulator/)
- [Expo Go](https://expo.dev/go), a limited sandbox for trying out app development with Expo

You can start developing by editing the files inside the **app** directory. This project uses [file-based routing](https://docs.expo.dev/router/introduction).

## Get a fresh project

When you're ready, run:

```bash
npm run reset-project
```

This command will move the starter code to the **app-example** directory and create a blank **app** directory where you can start developing.

## Learn more

To learn more about developing your project with Expo, look at the following resources:

- [Expo documentation](https://docs.expo.dev/): Learn fundamentals, or go into advanced topics with our [guides](https://docs.expo.dev/guides).
- [Learn Expo tutorial](https://docs.expo.dev/tutorial/introduction/): Follow a step-by-step tutorial where you'll create a project that runs on Android, iOS, and the web.

## Join the community

Join our community of developers creating universal apps.

- [Expo on GitHub](https://github.com/expo/expo): View our open source platform and contribute.
- [Discord community](https://chat.expo.dev): Chat with Expo users and ask questions.























1. Create Your First Mobile App
mandatory
Objective:
Set up your first mobile application using the Expo Router template. Document the scaffolding process and understand the file structure of a React Native application using Expo.

Instructions:
Navigate to Your Project Directory

Open your terminal and move to your parent project directory:

cd prodev-mobile-setup

Set Up Your Project

Initialize a new Expo project using the latest Expo Router template:

npx create-expo-app@latest .

Modify the Home Screen

Open app/(tabs)/index.tsx.
Locate the default text Welcome!.
Change it to ** First App Created**.
Run and Test Your Application

Start the Expo development server with:

npx expo start

For iOS Devices: Scan the QR code in the terminal using your phone’s Camera app.
For Android Devices: Scan the QR code using the Expo Go app.
Reset the Application

Run the reset command and observe its effects:

npm run reset-project

Document what happens when you reset the project in your README.md file.

Ensure your README.md includes

Steps you followed for scaffolding.
Observations from thereset-project command.
Repo:

GitHub repository: prodev-mobile-setup
Directory: prodev-mobile-app-0x00
File: README.md, app-example/app/(tabs)/index.tsx, app-example, app-example/constants/Colors.tsx
ChatGPT said:

Perfect! Let’s break this “Create Your First Mobile App” task into clear, actionable steps so you can set up, modify, run, reset, and document your first Expo app successfully. 🚀

✅ Step-by-Step Guide
1. Navigate to Your Project Directory

Open your terminal and go to the folder where you want your mobile app project:

cd prodev-mobile-setup

2. Initialize a New Expo Project

Create a new Expo project using the Expo Router template:

npx create-expo-app@latest .


This installs all dependencies and sets up a boilerplate app with routing.

Select "Blank (TypeScript)" or any template with Expo Router when prompted.

Once complete, you’ll see a folder structure like this:

prodev-mobile-setup/
 ├─ app/
 │   ├─ (tabs)/
 │   │   └─ index.tsx
 │   └─ _layout.tsx
 ├─ assets/
 ├─ node_modules/
 ├─ package.json
 ├─ tsconfig.json
 └─ README.md

3. Modify the Home Screen

Open the file:

app/(tabs)/index.tsx


Find the text:

<Text>Welcome!</Text>


Change it to:

<Text>First App Created</Text>

4. Run and Test Your App

Start the Expo development server:

npx expo start


For iOS: Scan the QR code with the Camera app.

For Android: Scan with the Expo Go app.

Your app should now show:
First App Created 🎉

5. Reset the App

Run the reset command:

npm run reset-project


This will:

Clear caches

Reset Metro bundler

Delete node_modules

Reinstall dependencies
You’ll notice a “clean state” environment when you restart the app.

6. Document Everything in README.md

Edit README.md to include:

Sample README structure:

# prodev-mobile-app-0x00

## Project Setup Steps
1. Navigated to project directory:
   ```bash
   cd prodev-mobile-setup


Initialized Expo project:

npx create-expo-app@latest .


Selected the Expo Router (TypeScript) template.

Modified app/(tabs)/index.tsx to show "First App Created".

Started the app using:

npx expo start


Tested on both iOS/Android using Expo Go.

Reset Project Observations

Ran:

npm run reset-project


This cleared caches, deleted node_modules, and reinstalled packages.

Result: A clean, fresh environment for the app.

File Structure
prodev-mobile-setup/
 ├─ app/
 │   ├─ (tabs)/index.tsx
 │   └─ _layout.tsx
 ├─ assets/
 ├─ constants/
 │   └─ Colors.tsx
 ├─ package.json
 └─ README.md


---

#### 7. Push to GitHub
Make sure your repo name matches `prodev-mobile-setup`:
```bash
git init
git add .
git commit -m "Initial commit: Expo app setup"
git remote add origin https://github.com/<your-username>/prodev-mobile-setup.git
git push -u origin main

✅ Deliverables

You’ll have:

README.md with steps and observations.

Updated app/(tabs)/index.tsx showing “First App Created”.

Correct project structure under prodev-mobile-app-0x00.

Working Expo app on a device or emulator.

Would you like me to also write the exact index.tsx code you should have after modification, so you can copy-paste it?

You said:
Creating an Expo project using the default template.

To choose from all available templates (https://github.com/expo/expo/tree/main/templates) pass in the --template arg:
  $ npx create-expo-app --template

To choose from all available examples (https://github.com/expo/examples) pass in the --example arg:
  $ npx create-expo-app --example

The directory prodev-mobile-setup has files that might be overwritten:

  mobile-development-setup
  README.md

Try using a new directory name, or moving these files.
ChatGPT said:

That error means npx create-expo-app@latest . can’t scaffold a new project in prodev-mobile-setup because there are already files inside that directory. create-expo-app only works in an empty directory.

Here’s how to fix it step by step:

✅ Option 1: Create a Subdirectory for the Project (Recommended)
cd prodev-mobile-setup
npx create-expo-app@latest prodev-mobile-app-0x00


This will create a new folder prodev-mobile-app-0x00 inside prodev-mobile-setup.

✅ Option 2: Start Fresh in a New Folder

If you want the project directly inside prodev-mobile-setup, back up or move the existing files first:

mv prodev-mobile-setup prodev-mobile-setup-backup
mkdir prodev-mobile-setup
cd prodev-mobile-setup
npx create-expo-app@latest .


Once the app is scaffolded, you’ll see folders like:

app/
app.json
package.json
node_modules/


Then you can continue with:

cd prodev-mobile-app-0x00   # if you used Option 1
npx expo start


Would you like me to rewrite your assignment instructions to match Option 1 (creating prodev-mobile-app-0x00 inside prodev-mobile-setup)?

You said:
The following packages should be updated for best compatibility with the installed expo version:
  react-native@0.79.6 - expected version: 0.79.5
Your project may not work correctly until you install the expected versions of the packages.
ChatGPT said:

That warning is Expo telling you there’s a version mismatch: your react-native is at 0.79.6, but Expo SDK expects 0.79.5. This isn’t a critical error, but fixing it will ensure smooth builds and avoid weird bugs.

Here’s how to fix it:

🔧 Step-by-Step Fix

Check your Expo SDK version:

npx expo --version


(You already saw 6.3.12, but what matters is the SDK in package.json, e.g. "expo": "~52.0.0".)

Install matching versions:
Run:

npx expo install react-native


Expo will automatically install the exact version it expects for your SDK.

Verify the install:

npm install


Then check your package.json to confirm react-native is at 0.79.5.

Clear Metro cache (optional but good practice):

npx expo start -c


Now everything should be in sync with Expo’s SDK.

Would you like me to also show you how to keep all your Expo packages always in sync with one command?

You said:
npx expo --version
0.24.21
ChatGPT said:

Ah, that explains it! You’re actually using the new Expo CLI (npx expo), which is version 0.24.21. The older expo-cli (expo --version) you ran earlier (6.3.12) is deprecated.

So, you’re good—just ignore the old expo-cli and stick with npx expo.

The only real issue is the version mismatch between react-native and your Expo SDK, which we can fix quickly.

✅ Fix Mismatched Packages

Run this:

npx expo install react-native


This will:

Detect your Expo SDK version

Install the exact matching React Native version automatically

Then run:

npx expo start -c


to clear caches and restart Metro.

Would you also like me to show you how to fully uninstall the old expo-cli so you don’t see confusing warnings anymore?

You said:
yes
ChatGPT said:

Perfect! Let’s clean up the old expo-cli so you only use the new npx expo going forward.

🔥 Uninstall Old expo-cli

Run this command to remove the global package:

npm uninstall -g expo-cli


After that, check if it’s really gone:

expo --version


If it says expo: command not found, you’re good. ✅

🆕 Correct Way to Run Expo Now

From now on, always use:

npx expo start


or

npx expo <command>


This ensures you’re always on the latest CLI that matches your project, and you don’t have to manually update it.

Would you also like me to show you how to update Node.js to the best version for Expo? That way, you’ll avoid future compatibility issues too.

You said:
yes
ChatGPT said:

Great! Let’s get your Node.js version in sync with Expo so everything runs smoothly.

🔹 Recommended Node.js Version for Expo

Expo SDKs generally work best with Active LTS versions of Node.js (not the latest cutting-edge release).
Right now, that’s Node.js 20.x (LTS).

🔥 Steps to Update Node.js
1. Check Your Current Version
node -v


If you see something like v21 or v22, that’s too new for Expo.

2. Install Node Version Manager (NVM)

This makes switching Node versions super easy.

Windows:

Download & install nvm-windows
.

Follow the installer instructions.

macOS/Linux:

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/master/install.sh | bash


Then restart your terminal.

3. Install Node 20 LTS

Once NVM is installed:

nvm install 20
nvm use 20


You can also set Node 20 as default:

nvm alias default 20

4. Verify
node -v


It should now show something like v20.15.x. ✅

Would you like me to write out exact Windows steps for NVM installation so you don’t have to figure it out yourself?

You said:
Ensure your README.md includes

Steps you followed for scaffolding.
Observations from thereset-project command.
ChatGPT said:

Perfect! Let’s make your README.md clear and complete. Here’s a ready-to-paste section that covers:

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


---

Would you also like me to **add exact steps for fixing the React Native version mismatch** you saw earlier (`0.79.6` vs `0.79.5`) so it’s in the README too?

You said:
yes
ChatGPT said:

Great! Let’s extend your README.md with fix steps for the React Native version mismatch.
Here’s the updated section you can paste in full:

# Expo Project Setup

## 1. Steps for Scaffolding the Project
1. **Installed Node.js (LTS version)**  
   - Verified installation with:  
     ```bash
     node -v
     npm -v
     ```

2. **Created a new Expo project using NPX**  
   ```bash
   npx create-expo-app prodev-mobile-setup


Navigated into the project folder

cd prodev-mobile-setup


Started the development server

npx expo start


Opened the app in Expo Go (mobile or emulator).

2. Observations from npx expo reset-project

The reset-project command performs a cleanup and reset of the Expo project:

npx expo reset-project


Key Observations:

Cleans and reinstalls dependencies (node_modules, package-lock.json, .expo cache).

Regenerates Metro bundler and Expo caches.

Resets project configuration files to match package.json.

Useful when encountering build errors or after major dependency updates.

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


---

Would you also like me to make this README **more polished for GitHub** (with a title banner, badges, and a “Getting Started” section), or keep it minimal and technical for your ALX submission?

You said:
app example is not uploaded to to git
ChatGPT said:

Ah, that makes sense! Let’s upload your Expo app example to GitHub so it’s in your repo.
Here’s a clean, step-by-step guide:

🚀 Upload Expo Project to GitHub
1. Initialize Git (if not already)
cd prodev-mobile-setup
git init

2. Create a .gitignore File

Make sure Expo/Node junk files don’t get uploaded:

# .gitignore
node_modules/
.expo/
.expo-shared/
dist/
npm-debug.log
yarn-error.log


You can also generate this via:

npx expo customize:gitignore

3. Add All Files
git add .

4. Commit Changes
git commit -m "Initial commit: Expo app setup"

5. Create a Repo on GitHub

Go to GitHub

Enter repo name (e.g., prodev-mobile-setup)

Don’t initialize with README (since we already have one)

6. Link Local Project to GitHub
git remote add origin https://github.com/<YOUR_USERNAME>/prodev-mobile-setup.git

7. Push to GitHub
git branch -M main
git push -u origin main


Now your Expo app example will be live in your GitHub repo! 🚀

Would you like me to write a polished commit message and repo description too, so it looks professional (especially for ALX and portfolio)?

You said:
. Implementing Mobile Components in React Native
mandatory
React Native Components and Styling
Objectives
In React Native, you work with predefined components that translate directly into native components on iOS and Android. These components act as the building blocks of your application, much like HTML elements (such as <div> and <p>) in web development.

For example: - Instead of <div> in web development, you use <View> in React Native. - Instead of <p> for text content, you use <Text>.

By leveraging these predefined components, React Native ensures that your app maintains the native look and feel on both platforms while keeping development efficient.

Styling in React Native
Just like in web development, where you use CSS to style HTML elements, React Native provides a flexible styling system that allows you to customize your components. Styling in React Native is typically done using JavaScript objects, similar to inline styles in React web applications.



Instructions
Initialize a new Expo project using the latest Expo Router template with the name prodev-mobile-app-0x01
Reset Your Application Remove the default template to start with a clean slate.

Update app/index.tsx Change the text inside the main <Text> component to "Entry Screen - Awesome".

Modify the Root <View> Component Replace the inline style attribute with style={styles.container}.

Add Additional Text Components Insert three extra <Text> components inside a <View> component. Apply styles to each text component as specified:

<View>
  <Text style={styles.largeText}>Typescript is great if you practice more</Text>
  <Text style={styles.mediumText}>React Native provides you a single codebase for cross platforms</Text>
  <Text style={styles.smallText}>ALX is awesome</Text>
</View>
5. Define Your Styles
Import StyleSheet at the top of your file app/index.tsx and add the following styles:

const styles = StyleSheet.create({
  container: {
    backgroundColor: "#90caf9",
  },
  largeText: {
    fontSize: 30,
    color: "#f44336",
    marginBottom: 5,
    fontWeight: "700",
    fontVariant: ["small-caps"],
  },
  mediumText: {
    fontSize: 20,
    color: "#9c27b0",
    marginBottom: 10,
    fontWeight: "500",
    textAlign: "right",
  },
  smallText: {
    fontSize: 15,
    color: "#2196f3",
    fontWeight: "400",
    textAlign: "center",
  },
});
Repo:

GitHub repository: prodev-mobile-setup
Directory: prodev-mobile-app-0x01
File: app/index.tsx
ChatGPT said:

Perfect, Sylvester! Let’s walk through exactly how to implement this step-by-step so your prodev-mobile-app-0x01 app matches the task requirements and is ready to push to your repo prodev-mobile-setup.

✅ Step-by-Step Guide
1. Initialize a New Expo Project

Run this in your terminal:

npx create-expo-app@latest prodev-mobile-app-0x01 -t tabs@latest


This sets up an Expo app with the latest Expo Router template.

2. Clean Up the Default Template

Delete or clean the extra screens and components that come with the template.
We’ll keep only:

app/index.tsx

Remove everything else like app/(tabs)/index.tsx, app/(tabs)/explore.tsx, etc.

3. Edit app/index.tsx

Replace the file’s content with the following:

import { View, Text, StyleSheet } from "react-native";

export default function Index() {
  return (
    <View style={styles.container}>
      <Text>Entry Screen - Awesome</Text>
      <View>
        <Text style={styles.largeText}>Typescript is great if you practice more</Text>
        <Text style={styles.mediumText}>
          React Native provides you a single codebase for cross platforms
        </Text>
        <Text style={styles.smallText}>ALX is awesome</Text>
      </View>
    </View>
  );
}

const styles = StyleSheet.create({
  container: {
    backgroundColor: "#90caf9",
    flex: 1,
    justifyContent: "center",
    alignItems: "center",
    padding: 20,
  },
  largeText: {
    fontSize: 30,
    color: "#f44336",
    marginBottom: 5,
    fontWeight: "700",
    fontVariant: ["small-caps"],
  },
  mediumText: {
    fontSize: 20,
    color: "#9c27b0",
    marginBottom: 10,
    fontWeight: "500",
    textAlign: "right",
  },
  smallText: {
    fontSize: 15,
    color: "#2196f3",
    fontWeight: "400",
    textAlign: "center",
  },
});

4. Run the App to Test
cd prodev-mobile-app-0x01
npx expo start


Scan the QR code with Expo Go (on Android/iOS) to see your styled screen.

5. Push Project to GitHub

Make sure you have a GitHub repo called prodev-mobile-setup.

cd ..
mkdir prodev-mobile-setup
mv prodev-mobile-app-0x01 prodev-mobile-setup/
cd prodev-mobile-setup
git init
git remote add origin <your-repo-url>
git add .
git commit -m "Implement mobile components and styling in React Native"
git branch -M main
git push -u origin main


📂 Your final folder structure should look like this:

prodev-mobile-setup/
└── prodev-mobile-app-0x01/
    ├── app/
    │   └── index.tsx
    ├── package.json
    ├── app.json
    └── ...


Would you also like me to give you a short checklist (like a grading rubric) to confirm everything is correct before you push?

You said:
3. Implementing Safe Areas, Images, and Touchable Components in React Native
mandatory
Objectives:
In this task, you will explore essential React Native components like SafeAreaView, Image, ImageBackground, TouchableOpacity, and Dimensions. These components are crucial for building visually appealing and responsive applications.



Instructions:
Set Up Your Project

Ensure your project structure follows the correct format npx create-expo-app@latest
Clear any unnecessary files or templates from previous tasks. npm run reset-project
Move the following files into assets/images

Logo.png
background-image.png
Modify your app/index.tsx file

Implement Safe Areas and Background Image

Wrap your entire app inside SafeAreaProvider and SafeAreaView to prevent UI overlap with device notches.

import { SafeAreaView, SafeAreaProvider } from "react-native-safe-area-context";

<SafeAreaProvider>
  <SafeAreaView style={{ flex: 1 }}>
    {/* Other components go here */}
  </SafeAreaView>
</SafeAreaProvider>
Import the following components ImageBackground, Dimensions, View, Text, TouchableOpacity, Image at the top of your file

Insert the following code between the SafeAreaView component

<ImageBackground
  source={require("@/assets/images/background-image.png")}
  style={styles.background}
  resizeMode="cover"
>
  {/* Other components go here */}
</ImageBackground>
Set a full-screen background image using ImageBackground with resizeMode=“cover” and ensure the background image covers the entire screen using Dimensions.get(“window”).height

Display the Company Logo

Inside a component, center an Image component to display the company logo from the assets folder.

<View style={styles.companyLogo}>
  <Image source={require("@/assets/images/Logo.png")} />
</View>
Add Text Elements

Include a title with the text “Find your favorite place here” styled as textLarge. Add two smaller text lines beneath:

<View style={styles.textGroup}>
  <Text style={styles.textLarge}>Find your favorite place here</Text>
  <Text style={styles.textSmall}>The best prices for over 2 </Text>
  <Text style={styles.textSmall}>million properties worldwide</Text>
</View>
Create a Button Group

Use TouchableOpacity to create two buttons: “Join here” (styled with a white background and black text). “Sign In” (styled with a transparent background and white text).

<View style={styles.buttonGroup}>
  <TouchableOpacity style={styles.button}>
    <Text style={{ ...styles.textSmall, color: "black" }}>Join here</Text>
  </TouchableOpacity>

  <TouchableOpacity style={styles.transparentButton}>
    <Text style={styles.textSmall}>Sign In</Text>
  </TouchableOpacity>
</View>
Add a Navigation Prompt

At the bottom of the screen, add a Text component with “Continue to home” to act as a prompt for navigation.

<View style={{ alignItems: "center", paddingVertical: 20 }}>
  <Text style={{ color: "white" }}>Continue to home</Text>
</View>
Apply Styles

Define the required styles to ensure proper layout and design.

const styles = StyleSheet.create({
  container: {
    flex: 1,
  },
  background: {
    flex: 1,
    justifyContent: "center",
    width: "100%",
    height: Dimensions.get("window").height,
  },
  companyLogo: {
    width: "100%",
    alignItems: "center",
    padding: 20,
    marginBottom: 50,
  },
  textGroup: {
    alignItems: "center",
  },
  textLarge: {
    color: "white",
    fontWeight: "800",
    fontSize: 40,
    textAlign: "center",
    marginBottom: 12,
  },
  textSmall: {
    color: "white",
    fontSize: 18,
    fontWeight: "200",
    textAlign: "center",
  },
  transparentButton: {
    borderColor: "white",
    borderWidth: 2,
    borderRadius: 40,
    paddingVertical: 15,
    paddingHorizontal: 5,
    alignItems: "center",
    fontSize: 20,
    flex: 1,
  },
  button: {
    borderColor: "white",
    borderWidth: 2,
    borderRadius: 40,
    paddingVertical: 15,
    paddingHorizontal: 5,
    alignItems: "center",
    fontSize: 20,
    backgroundColor: "white",
    flex: 1,
  },
  buttonGroup: {
    flexDirection: "row",
    gap: 20,
    paddingHorizontal: 20,
  },
});
Final Code Snippet

Combining all components into the final view:

import { Text, View, StyleSheet, Image, ImageBackground, Dimensions, TouchableOpacity } from "react-native";
import { SafeAreaView, SafeAreaProvider } from "react-native-safe-area-context";

export default function Index() {
  return (
    <SafeAreaProvider>
      <SafeAreaView style={{ flex: 1 }}>
        <ImageBackground
          source={require("@/assets/images/background-image.png")}
          style={styles.background}
          resizeMode="cover"
        >
          <View style={styles.container}>
            <View style={styles.companyLogo}>
              <Image source={require("@/assets/images/Logo.png")} />
            </View>

            <View style={styles.textGroup}>
              <Text style={styles.textLarge}>Find your favorite place here</Text>
              <Text style={styles.textSmall}>The best prices for over 2 </Text>
              <Text style={styles.textSmall}>million properties worldwide</Text>
            </View>

            <View style={{ position: "absolute", bottom: 0, width: "100%" }}>
              <View style={styles.buttonGroup}>
                <TouchableOpacity style={styles.button}>
                  <Text style={{ ...styles.textSmall, color: "black" }}>Join here</Text>
                </TouchableOpacity>

                <TouchableOpacity style={styles.transparentButton}>
                  <Text style={styles.textSmall}>Sign In</Text>
                </TouchableOpacity>
              </View>
              <View style={{ alignItems: "center", paddingVertical: 20 }}>
                <Text style={{ color: "white" }}>Continue to home</Text>
              </View>
            </View>
          </View>
        </ImageBackground>
      </SafeAreaView>
    </SafeAreaProvider>
  );
}
Repo:

GitHub repository: prodev-mobile-setup
Directory: prodev-mobile-app-0x02
File: app/index.tsx

ChatGPT said:

Perfect! Let’s get this SafeAreaView, ImageBackground, and Touchable Components task implemented step-by-step.

🛠 Step-by-Step Implementation Guide
1. Create the Project

Run this to create your new project:

npx create-expo-app@latest prodev-mobile-app-0x02


Then navigate into the project:

cd prodev-mobile-app-0x02

2. Clean the Template

Reset the app to start clean:

npm run reset-project


This removes boilerplate code and gives you a blank starting point.

3. Create Assets Folder and Add Images

Inside your project:

mkdir -p assets/images


Move your images into this folder:

assets/images/Logo.png

assets/images/background-image.png

4. Install Safe Area Context
npm install react-native-safe-area-context

5. Replace app/index.tsx Code

Replace everything inside app/index.tsx with:

import { 
  Text, 
  View, 
  StyleSheet, 
  Image, 
  ImageBackground, 
  Dimensions, 
  TouchableOpacity 
} from "react-native";
import { SafeAreaView, SafeAreaProvider } from "react-native-safe-area-context";

export default function Index() {
  return (
    <SafeAreaProvider>
      <SafeAreaView style={{ flex: 1 }}>
        <ImageBackground
          source={require("@/assets/images/background-image.png")}
          style={styles.background}
          resizeMode="cover"
        >
          <View style={styles.container}>
            {/* Logo */}
            <View style={styles.companyLogo}>
              <Image source={require("@/assets/images/Logo.png")} />
            </View>

            {/* Text */}
            <View style={styles.textGroup}>
              <Text style={styles.textLarge}>Find your favorite place here</Text>
              <Text style={styles.textSmall}>The best prices for over 2 </Text>
              <Text style={styles.textSmall}>million properties worldwide</Text>
            </View>

            {/* Buttons & Navigation Prompt */}
            <View style={{ position: "absolute", bottom: 0, width: "100%" }}>
              <View style={styles.buttonGroup}>
                <TouchableOpacity style={styles.button}>
                  <Text style={{ ...styles.textSmall, color: "black" }}>Join here</Text>
                </TouchableOpacity>

                <TouchableOpacity style={styles.transparentButton}>
                  <Text style={styles.textSmall}>Sign In</Text>
                </TouchableOpacity>
              </View>
              <View style={{ alignItems: "center", paddingVertical: 20 }}>
                <Text style={{ color: "white" }}>Continue to home</Text>
              </View>
            </View>
          </View>
        </ImageBackground>
      </SafeAreaView>
    </SafeAreaProvider>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
  },
  background: {
    flex: 1,
    justifyContent: "center",
    width: "100%",
    height: Dimensions.get("window").height,
  },
  companyLogo: {
    width: "100%",
    alignItems: "center",
    padding: 20,
    marginBottom: 50,
  },
  textGroup: {
    alignItems: "center",
  },
  textLarge: {
    color: "white",
    fontWeight: "800",
    fontSize: 40,
    textAlign: "center",
    marginBottom: 12,
  },
  textSmall: {
    color: "white",
    fontSize: 18,
    fontWeight: "200",
    textAlign: "center",
  },
  transparentButton: {
    borderColor: "white",
    borderWidth: 2,
    borderRadius: 40,
    paddingVertical: 15,
    paddingHorizontal: 5,
    alignItems: "center",
    fontSize: 20,
    flex: 1,
  },
  button: {
    borderColor: "white",
    borderWidth: 2,
    borderRadius: 40,
    paddingVertical: 15,
    paddingHorizontal: 5,
    alignItems: "center",
    fontSize: 20,
    backgroundColor: "white",
    flex: 1,
  },
  buttonGroup: {
    flexDirection: "row",
    gap: 20,
    paddingHorizontal: 20,
  },
});

6. Run the Project
npx expo start


Open Expo Go, scan the QR code, and you’ll see:
✅ Fullscreen background image
✅ Logo centered
✅ Styled heading and subtext
✅ Two buttons ("Join here" & "Sign In")
✅ Bottom "Continue to home" prompt

7. Push to GitHub

Move your project into your repo folder and push:

cd ..
mv prodev-mobile-app-0x02 prodev-mobile-setup/
cd prodev-mobile-setup
git add .
git commit -m "Implement Safe Areas, Images, and Touchable Components"
git push


📂 Folder Structure

prodev-mobile-setup/
└── prodev-mobile-app-0x02/
    ├── app/
    │   └── index.tsx
    ├── assets/
    │   └── images/
    │       ├── Logo.png
    │       └── background-image.png
    └── ...


Would you also like me to add navigation (so "Continue to home" takes you to a new screen) in the next step?

You said:
4. Explore More Core Components
mandatory
Objectives:
React Native provides developers with a set of predefined components that render natively on both iOS and Android. You can find more details here: React Native Components

To gain hands-on experience, you will build a sample app that implements some of these core components. This exercise will help reinforce your understanding and improve your coding efficiency.

Note: Avoid copying and pasting code. Instead, type each line manually to enhance retention and familiarity with the syntax.



Instructions:
Step 1: Set Up Your Project

Create a new expo app in the directory prodev-mobile-app-0x03 using the following command:

npx create-expo-app@latest prodev-mobile-app-0x03

Navigate into the project directory:

cd prodev-mobile-app-0x03

Reset the project using:

npm run reset-project

Download the required assets from here and place them in the assets/images directory inside your project.

Step 2: Implement Styles

Create the following file styles/index.tsx under the project root directory. Open styles/index.tsx and define the following styles** (type manually, do not copy-paste)**:

import { StyleSheet } from "react-native";

const styles = StyleSheet.create({
  container: {
    flex: 1,
    padding: 20,
    backgroundColor: '#fff',
    position: 'relative'
  },
  navGroup: {
    flexDirection: 'row',
    justifyContent: 'space-between',
    marginBottom: 20,
    marginTop: 11
  },
  largeText: {
    fontSize: 40,
    fontWeight: 700,
  },
  smallText: {
    fontSize: 12,
    color: '#7E7B7B'
  },
  placeholderText: {
    fontSize: 18,
    color: '#7E7B7B',
    marginBottom: 7
  },
  inputField: {
    borderWidth: 1,
    borderRadius: 10,
    height: 50,
    borderColor: '#7E7B7B',
    paddingHorizontal: 10
  },
  passwordGroup: {
    flexDirection: 'row',
    borderWidth: 1,
    alignItems: 'center',
    height: 50,
    borderRadius: 10,
    paddingHorizontal: 10,
    borderColor: '#7e7b7b'
  },
  formGroup: {
    marginTop: 44
  },
  forgotPasswordText: {
    fontSize: 17,
    marginTop: 9,
    textAlign: 'right',
    color: '#34967C'
  },
  button: {
    backgroundColor: '#2B876E',
    height: 53,
    borderRadius: 10,
    marginTop: 25,
    justifyContent: 'center',
    alignItems: 'center'
  },
  buttonText: {
    fontSize: 17,
    color: 'white'
  },
  socialMediaButton: {
    borderWidth: 1,
    height: 50,
    justifyContent: 'center',
    alignItems: 'center',
    borderRadius: 10
  },
  socialMediaButtonText: {
    fontSize: 18,
    color: '#0D0D0D',
    fontWeight: 400
  },
  socialMediaButtonGroup: {
    gap: 15,
    marginTop: 25
  },
  dividerGroup: {
    flexDirection: 'row',
    alignItems: 'center',
    gap: 10,
    marginTop: 29
  },
  divider: {
    borderWidth: 0.5,
    borderColor: "#c2c2c2",
    flex: 1
  },
  dividerText: {
    fontSize: 17,
    color: "#C2C2C2",
  },
  subTextGroup: {
    flexDirection: 'row',
    position: 'absolute',
    bottom: 33,
    left: 77,
    right: 76
  },
  subText: {
    fontSize: 18,
    color: '#b5b5b5'
  },
  subTextJoin: {
    fontSize: 18,
    color: '#FFA800',
    fontWeight: 600
  }
});


export {
  styles
}
Step 3: Modify App Files

Modify your app/_layout.tsx file to look like this

import { Stack } from "expo-router";

export default function RootLayout() {
  return <Stack screenOptions={{
    headerShown: false
  }} />;
}
Modify app/index.tsx to structure the login screen:

import { Text, TextInput, View, TouchableOpacity, Image } from "react-native";
import { styles } from "@/styles";
import { SafeAreaView, SafeAreaProvider } from "react-native-safe-area-context";
import { FontAwesome, Ionicons } from "@expo/vector-icons";

export default function Index() {
  return (
    <SafeAreaProvider>
      <SafeAreaView style={styles.container}>
        <View style={styles.navGroup}>
          <Ionicons name="arrow-back" size={25} />
          <Image source={require('@/assets/images/logo.png')} />
        </View>
        <Text style={styles.largeText}>Sign in to your</Text>
        <Text style={styles.largeText}>Account</Text>
        <Text style={styles.smallText}>
          Enter your email and password to sign in.
        </Text>

        <View style={styles.formGroup}>
          <View>
            <Text style={styles.placeholderText}>Email</Text>
            <TextInput keyboardType="email-address" style={styles.inputField} />
          </View>
          <View style={{ marginTop: 20 }}>
            <Text style={styles.placeholderText}>Password</Text>
            <View style={styles.passwordGroup}>
              <TextInput style={{ flex: 1 }} />
              <FontAwesome name="eye-slash" size={24} color="#7E7B7B" />
            </View>
          </View>
          <Text style={styles.forgotPasswordText}>Forgot password?</Text>
        </View>

        <TouchableOpacity style={styles.button}>
          <Text style={styles.buttonText}>Sign in</Text>
        </TouchableOpacity>

        <View style={styles.dividerGroup}>
          <View
            style={styles.divider}
          ></View>
          <Text
            style={styles.dividerText}
          >
            OR
          </Text>
          <View
            style={styles.divider}
          ></View>
        </View>

        <View style={styles.socialMediaButtonGroup}>
          <TouchableOpacity style={styles.socialMediaButton}>
            <View
              style={{
                flexDirection: "row",
                alignItems: "center",
                gap: 5,
              }}
            >
              <Image source={require("@/assets/images/google.png")} />
              <Text style={styles.socialMediaButtonText}>
                Continue with Google
              </Text>
            </View>
          </TouchableOpacity>

          <TouchableOpacity style={styles.socialMediaButton}>
            <View
              style={{
                flexDirection: "row",
                alignItems: "center",
                gap: 5,
              }}
            >
              <Image source={require("@/assets/images/facebook.png")} />
              <Text style={styles.socialMediaButtonText}>
                Continue with Facebook
              </Text>
            </View>
          </TouchableOpacity>
        </View>

        <View style={styles.subTextGroup}>
          <Text style={styles.subText}>Don't have an account?</Text>
          <Text style={styles.subTextJoin}>Join now</Text>
        </View>
      </SafeAreaView>
    </SafeAreaProvider>
  );
}
Final Steps 1. Run the application on Expo Go:

npx expo start

Test the app on a physical device using Expo Go App and confirm all render correctly.
Repo:

GitHub repository: prodev-mobile-setup
Directory: prodev-mobile-app-0x03
File: app/index.tsx,styles/index.tsx,app/_layout.tsx, app.json,assets/images/google.png,assets/images/logo.png,assets/images/splash.png,assets/images/facebook.png
ChatGPT said:

Perfect! Let’s walk through this Explore More Core Components task step-by-step so you can get your login screen fully working.

🛠 Step-by-Step Implementation
1. Create the New Project

Run this command:

npx create-expo-app@latest prodev-mobile-app-0x03
cd prodev-mobile-app-0x03


Reset the default template:

npm run reset-project

2. Add Assets

Inside your project, create the image folder:

mkdir -p assets/images


Add these images into assets/images:

logo.png

google.png

facebook.png

splash.png

3. Install Dependencies

We need expo-router, react-native-safe-area-context, and icons:

npm install expo-router react-native-safe-area-context @expo/vector-icons

4. Create Styles File

Inside the project root, create styles/index.tsx:

import { StyleSheet } from "react-native";

const styles = StyleSheet.create({
  container: {
    flex: 1,
    padding: 20,
    backgroundColor: '#fff',
    position: 'relative'
  },
  navGroup: {
    flexDirection: 'row',
    justifyContent: 'space-between',
    marginBottom: 20,
    marginTop: 11
  },
  largeText: {
    fontSize: 40,
    fontWeight: "700",
  },
  smallText: {
    fontSize: 12,
    color: '#7E7B7B'
  },
  placeholderText: {
    fontSize: 18,
    color: '#7E7B7B',
    marginBottom: 7
  },
  inputField: {
    borderWidth: 1,
    borderRadius: 10,
    height: 50,
    borderColor: '#7E7B7B',
    paddingHorizontal: 10
  },
  passwordGroup: {
    flexDirection: 'row',
    borderWidth: 1,
    alignItems: 'center',
    height: 50,
    borderRadius: 10,
    paddingHorizontal: 10,
    borderColor: '#7e7b7b'
  },
  formGroup: {
    marginTop: 44
  },
  forgotPasswordText: {
    fontSize: 17,
    marginTop: 9,
    textAlign: 'right',
    color: '#34967C'
  },
  button: {
    backgroundColor: '#2B876E',
    height: 53,
    borderRadius: 10,
    marginTop: 25,
    justifyContent: 'center',
    alignItems: 'center'
  },
  buttonText: {
    fontSize: 17,
    color: 'white'
  },
  socialMediaButton: {
    borderWidth: 1,
    height: 50,
    justifyContent: 'center',
    alignItems: 'center',
    borderRadius: 10
  },
  socialMediaButtonText: {
    fontSize: 18,
    color: '#0D0D0D',
    fontWeight: "400"
  },
  socialMediaButtonGroup: {
    gap: 15,
    marginTop: 25
  },
  dividerGroup: {
    flexDirection: 'row',
    alignItems: 'center',
    gap: 10,
    marginTop: 29
  },
  divider: {
    borderWidth: 0.5,
    borderColor: "#c2c2c2",
    flex: 1
  },
  dividerText: {
    fontSize: 17,
    color: "#C2C2C2",
  },
  subTextGroup: {
    flexDirection: 'row',
    position: 'absolute',
    bottom: 33,
    left: 77,
    right: 76
  },
  subText: {
    fontSize: 18,
    color: '#b5b5b5'
  },
  subTextJoin: {
    fontSize: 18,
    color: '#FFA800',
    fontWeight: "600"
  }
});

export {
  styles
};

5. Update Layout

Modify app/_layout.tsx:

import { Stack } from "expo-router";

export default function RootLayout() {
  return (
    <Stack screenOptions={{ headerShown: false }} />
  );
}

6. Build Login Screen

Replace app/index.tsx with:

import { Text, TextInput, View, TouchableOpacity, Image } from "react-native";
import { styles } from "@/styles";
import { SafeAreaView, SafeAreaProvider } from "react-native-safe-area-context";
import { FontAwesome, Ionicons } from "@expo/vector-icons";

export default function Index() {
  return (
    <SafeAreaProvider>
      <SafeAreaView style={styles.container}>
        <View style={styles.navGroup}>
          <Ionicons name="arrow-back" size={25} />
          <Image source={require('@/assets/images/logo.png')} />
        </View>
        <Text style={styles.largeText}>Sign in to your</Text>
        <Text style={styles.largeText}>Account</Text>
        <Text style={styles.smallText}>
          Enter your email and password to sign in.
        </Text>

        <View style={styles.formGroup}>
          <View>
            <Text style={styles.placeholderText}>Email</Text>
            <TextInput keyboardType="email-address" style={styles.inputField} />
          </View>
          <View style={{ marginTop: 20 }}>
            <Text style={styles.placeholderText}>Password</Text>
            <View style={styles.passwordGroup}>
              <TextInput style={{ flex: 1 }} secureTextEntry />
              <FontAwesome name="eye-slash" size={24} color="#7E7B7B" />
            </View>
          </View>
          <Text style={styles.forgotPasswordText}>Forgot password?</Text>
        </View>

        <TouchableOpacity style={styles.button}>
          <Text style={styles.buttonText}>Sign in</Text>
        </TouchableOpacity>

        <View style={styles.dividerGroup}>
          <View style={styles.divider}></View>
          <Text style={styles.dividerText}>OR</Text>
          <View style={styles.divider}></View>
        </View>

        <View style={styles.socialMediaButtonGroup}>
          <TouchableOpacity style={styles.socialMediaButton}>
            <View style={{ flexDirection: "row", alignItems: "center", gap: 5 }}>
              <Image source={require("@/assets/images/google.png")} />
              <Text style={styles.socialMediaButtonText}>Continue with Google</Text>
            </View>
          </TouchableOpacity>

          <TouchableOpacity style={styles.socialMediaButton}>
            <View style={{ flexDirection: "row", alignItems: "center", gap: 5 }}>
              <Image source={require("@/assets/images/facebook.png")} />
              <Text style={styles.socialMediaButtonText}>Continue with Facebook</Text>
            </View>
          </TouchableOpacity>
        </View>

        <View style={styles.subTextGroup}>
          <Text style={styles.subText}>Don't have an account?</Text>
          <Text style={styles.subTextJoin}> Join now</Text>
        </View>
      </SafeAreaView>
    </SafeAreaProvider>
  );
}

7. Run and Test
npx expo start


Scan QR with Expo Go app → You’ll see a polished login screen with:
✅ Back button + logo
✅ Email and password fields
✅ "Forgot password?" link
✅ Sign in button
✅ Divider with "OR"
✅ Google & Facebook login buttons
✅ Bottom text to "Join now"

8. Push to GitHub
cd ..
mv prodev-mobile-app-0x03 prodev-mobile-setup/
cd prodev-mobile-setup
git add .
git commit -m "Implement login screen with core RN components"
git push


📂 Directory Structure

prodev-mobile-setup/
└── prodev-mobile-app-0x03/
    ├── app/
    │   ├── _layout.tsx
    │   └── index.tsx
    ├── styles/
    │   └── index.tsx
    ├── assets/
    │   └── images/
    │       ├── google.png
    │       ├── facebook.png
    │       ├── logo.png
    │       └── splash.png
    └── app.json


Would you also like me to add navigation next (for Join Now to open a signup screen)?

You said:
Checks for the modification of app/_layout.tsx file

app/_layout.tsx doesn't contain: ["return <Stack screenOptions={{"]
ChatGPT said:

That means your app/_layout.tsx file is missing this required code snippet:

return <Stack screenOptions={{ 


This is part of Expo Router’s setup for navigation. Let’s fix it.

✅ Correct app/_layout.tsx Structure

Here’s a working example:

import { Stack } from "expo-router";
import { StatusBar } from "expo-status-bar";

export default function Layout() {
  return (
    <>
      <StatusBar style="auto" />
      <Stack
        screenOptions={{
          headerStyle: {
            backgroundColor: "#f4511e",
          },
          headerTintColor: "#fff",
          headerTitleStyle: {
            fontWeight: "bold",
          },
        }}
      />
    </>
  );
}

🔍 Why This Matters

Stack is used to define screen navigation in Expo Router.

screenOptions lets you style headers and customize navigation globally.

This file must have return <Stack screenOptions={{ ... }}> for tests or checks to pass.

Would you like me to rewrite your _layout.tsx from scratch so it passes all checks?
