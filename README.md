# Installation WebdriverIO for Mobile Testing

This project is a WebdriverIO setup for end-to-end mobile testing with Cucumber framework.

## Required
- [Android Studio](https://developer.android.com/studio)
- [Visual Studio Code](https://code.visualstudio.com/download)
- [Node JS](NodeJS)
- [Javasdk](https://www.oracle.com/java/technologies/downloads)
- Appium server install with command
    ```sh
    npm install -g appium
    ```
- APKTesting

## Steps
1. Install **Android Studio**, **Visual Studio**, **Node JS**, **JAVA**

2. Set up Virtual Device, open android Studio, click configure, click AVD Manager, add Virtual Devices

3.  Set Path for **JAVA_HOME**, for path default JAVA path install commonly in **C:\Program Files (x86)**, setting Environment Variables with the following:
    - Right click **This PC** atau **My Computer**
    - Select **Properties**
    - Click **Advanced system settings**
    - Click **Environment Variables**
    - In **System Variables**, click **New**
    - Add variable **JAVA_HOME**:
        - Variable name: **JAVA_HOME**
        - Variable value: Path instalation JDK (ex: **C:\Program Files\Java\jdk-17**)
    - Edit variable **Path**:
        - Click **Path**, then **Edit**
        - Click **New**
        - Add **%JAVA_HOME%\bin**
        - Click **OK**

4. Set Path for **ANDROID_HOME**, the path can be seen by open the **Android Studio** -> click **Configure** -> **SDK Manager**, then look at the Android SDK Location
    - How to search **Android SDK** location:
        - Commonly it is placed in: **C:\Users\[UserName]\AppData\Local\Android\Sdk**
        - Or, please check in **Android Studio**:
            1. Open **Android Studio**
            2. Open **Settings** (Ctrl + Alt + S)
            3. Search **Android SDK** on the left panel
            4. See **Android SDK Location**

    - Setting Environment Variables:
        - Right click **This PC** or **My Computer**
        - Select **Properties**
        - Click **Advanced system settings**
        - Click **Environment Variables**

    - Add new System Variable:
        - Click **New** in **System Variables**
        - Variable name: ANDROID_HOME
        - Variable value: Path Android SDK (ex: C:\Users\[UserName]\AppData\Local\Android\Sdk)
    
    -  Add Path for Platform Tools:
        - In **System Variables**, cari variable **Path**
        - Click **Edit**
        - Click **New**

    -  Add the following entries:
        -   ```sh
            %ANDROID_HOME%\platform-tools
            ```
        -   ```sh
            %ANDROID_HOME%\tools
            ```
        -   ```sh
            %ANDROID_HOME%\tools\bin
            ```

    - Setting verification:
        - Open new Command Prompt
        - Type commands: echo **%ANDROID_HOME%**
        - Check adb version
            ```sh
            adb --version
            ```
        - If the location of ANDROID_HOME and ADB version, then the setting is success

    - After setting ANDROID_HOME:
        1. Able to use ADB (Android Debug Bridge)
        2. Appium can detect Android SDK
        3. Able to run automated testing for Android