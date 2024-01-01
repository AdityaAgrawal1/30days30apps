# Genesis: Hello World App

## Overview
Welcome to "Genesis," the first project in your Android development journey. This "Hello World" app serves as an introduction to Android Studio, Jetpack Compose, and the basics of app development.

## Getting Started
### Prerequisites
- Android Studio Arctic Fox or later.
- Basic knowledge of Kotlin programming language.
- A computer capable of running Android Studio and emulator.

### Setting Up Android Studio and Project
1. **Install Android Studio**
   - Download Android Studio from the [official website](https://developer.android.com/studio).
   - Follow the installation instructions for your operating system.

2. **Create a New Project**
   - Launch Android Studio and select "New Project."
   - Choose the "Empty Compose Activity" template.
   - Name your project Genesis.
   - Ensure Kotlin is selected as the language.
   - Choose a minimum API level (API 21 or higher is recommended).
   - Finish the setup and wait for Android Studio to build the project.

### Understanding the Project Structure
- **MainActivity.kt**: The main entry point of your app. It contains the setup for your UI and any logic for the main screen.
- **/ui/theme**: Contains theming for your app, including color schemes and typography.
- **AndroidManifest.xml**: The manifest file that declares the app's configuration and activities.
- **Gradle Files**:
  - *build.gradle (Module)*: Specifies app-level dependencies and configurations.
  - *build.gradle (Project)*: Contains configurations that apply to your entire project.

### Jetpack Compose - Modern UI Toolkit
Jetpack Compose simplifies UI development in Android with a declarative approach. It allows developers to build native UIs in a more intuitive and flexible way compared to traditional XML.

#### Key Concepts
- **@Composable Functions**: These functions let you define your UI components. Anything that draws to the screen is a composable function.
- **Material Design**: Compose is integrated with Material Design for building aesthetically pleasing UIs.

## Running the App
1. Connect an Android device to your computer or set up an emulator in Android Studio.
2. Select the device from the dropdown menu in Android Studio.
3. Click the "Run" button to build and run the app on your device or emulator.

## The "Hello World" App in Compose
In `MainActivity.kt`, the `setContent` block sets up the UI for the app. The `Greeting` composable function is defined to display "Hello World" on the screen.

## MainActivity Class:

- `setContent { ... }`: Sets up the content of the activity using Jetpack Compose.
- `GenesisTheme { ... }`: Applies the custom theme (`GenesisTheme`) to the entire activity.

## Greeting Composable Function:

- `Box`: A composable that allows you to stack and align elements.
- `Text`: Displays text on the screen.
  - `text = "Hello World"`: The text content.
  - `fontWeight = FontWeight.Bold`: Specifies bold font weight for the text.
  - `modifier = modifier`: Accepts additional modifiers for styling.

## GreetingPreview Composable Function:

- `@Preview(showBackground = true)`: Generates a preview of the `Greeting` composable for design preview in Android Studio.
