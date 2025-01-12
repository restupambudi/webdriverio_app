# WebdriverIO App

This project is a WebdriverIO setup for end-to-end testing with Cucumber framework.

## Required
- [Android Studio](https://developer.android.com/studio)
- [Visual Studio Code](https://code.visualstudio.com/download)
- [Node JS](NodeJS)
- [Javasdk](https://www.oracle.com/java/technologies/downloads)
- Appiumserver install with command
    ```sh
    npm install -g appium
    ```
- APKTesting

1. Install Android Studio, Visual Studio, Node JS, JAVA
2. Set up Virtual Device, open android Studio, click configure, click AVD Manager, add Virtual Devices
3.  Set Path for JAVA_HOME, for path default JAVA path install commonly in C:\Program Files (x86)\, setting Environment Variables with the following:
    - Right click "This PC" atau "My Computer"
    - Select "Properties"
    - Click "Advanced system settings"
    - Click "Environment Variables"
    - In "System Variables", click "New"
    - Add variable JAVA_HOME:
        - Variable name: JAVA_HOME
        - Variable value: Path instalation JDK (ex: C:\Program Files\Java\jdk-17)
    - Editvariable "Path":
        - Klik "Path" lalu "Edit"
        - Klik "New"
        - Tambahkan: %JAVA_HOME%\bin
        - Klik OK
4. Set Path untuk ANDROID_HOME, untuk path bisa dilihat dengan cara, buka android studio-> Klik Configure-> SDK Manager dan kalian akan melihat Android SDK Location