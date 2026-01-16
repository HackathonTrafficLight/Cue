# Cue App Blueprint

## 🚀 Overview

**Cue** is a mobile application designed to solve the problem of waiting in line. It allows users to join a virtual queue, get real-time updates on their wait time, and receive a notification when it's their turn. The goal is to create a seamless and stress-free waiting experience.

This document outlines the project's features, design guidelines, and the plan for the current development phase.

---

## ✨ Features & Design (Version 1.0)

This section documents all the features and design choices implemented in the application, from the initial version to the current one.

### Core Features:
*   **Google Sign-In:** Users can sign in using their Google account for a quick and secure authentication process.

### UI/UX & Design:
*   **Login Screen:**
    *   **Layout:** A clean, centered layout featuring the app logo, a welcoming headline, and a prominent Google Sign-in button.
    *   **Logo:** The app's logo is displayed at the top (`assets/images/logo.png`).
    *   **Typography:** Modern and readable fonts from the `google_fonts` package are used.
        *   Headline ("Ready, Que!"): `GoogleFonts.inter`, 32pt, Bold.
        *   Sub-headline ("Leave it to us 🤷"): `GoogleFonts.inter`, 16pt, Regular.
        *   Button Text ("Sign in with Google"): `GoogleFonts.inter`, 18pt, Semi-Bold.
    *   **Color Scheme:** A simple and clean black and white theme.
    *   **Google Sign-In Button:** A full-width button with rounded corners, featuring the Google logo (`assets/images/google_logo.png`) for clear brand recognition.

### Technical Implementation:
*   **Project Structure:**
    *   `assets/images/`: Folder created to store image assets.
    *   `lib/login_screen.dart`: The main UI for the login screen.
*   **Dependencies:**
    *   `google_fonts`: Added for custom typography.
*   **Asset Registration:** The `assets/images/` directory is registered in `pubspec.yaml` to make the images available in the app.

---

## 📝 Current Plan: Initial Setup & Login Screen

This section outlines the plan and steps for the *current* requested change.

### Goal: Create the initial app structure and a visually appealing login screen as per the provided image.

**Plan & Steps:**

1.  **Project Initialization & Renaming:**
    *   ✅ Create a new Flutter project.
    *   ✅ Rename the project directory to `cue`.

2.  **Asset Folder Creation:**
    *   ✅ Create an `assets/images` folder to store app images.

3.  **Add Dependencies:**
    *   ✅ Add the `google_fonts` package to `pubspec.yaml` for custom fonts.

4.  **Create Login Screen UI:**
    *   ✅ Create a new file `lib/login_screen.dart`.
    *   ✅ Implement the UI using `StatelessWidget`.
    *   ✅ Add the app logo (`Image.asset('assets/images/logo.png')`).
    *   ✅ Add the headline "Ready, Que!" and sub-headline "Leave it to us 🤷" using `Text` and `GoogleFonts`.
    *   ✅ Create the "Sign in with Google" button using `ElevatedButton`, including the Google logo (`Image.asset('assets/images/google_logo.png')`).

5.  **Set Login Screen as Initial Route:**
    *   ✅ Modify `lib/main.dart`.
    *   ✅ Remove the default `MyHomePage` boilerplate code.
    *   ✅ Set `home` property of `MaterialApp` to `const LoginScreen()`.
    *   ✅ Hide the debug banner (`debugShowCheckedModeBanner: false`).

6.  **Register Assets in `pubspec.yaml`:**
    *   ✅ Update `pubspec.yaml` to include the `assets/images/` directory under the `flutter` section.

7.  **Create Blueprint:**
    *   ✅ Create this `blueprint.md` file to document the project and the work done.
