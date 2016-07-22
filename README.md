# android_monkey_test
## Overview
This is a python project for Android app autonomic test, based on `sdk tools`. It can install apks, running apps and take screenshots automatically. 
Through screenshots you can easily and quickly judge which app is suitable for you.
## Requirements
Python 2.6 or up

Android sdk

Downloaded apks

ps:you can download apk by app crawler [@https://github.com/mssun/android-apps-crawler](https://github.com/mssun/android-apps-crawler)
## Usage
* Use `aapt` to resolve apk and save apkInfo into txt(Remember to add your apk absolute path):

    ```
    python aaptOutput.py [apkDir]
    ```
For example, on windows. The command is like `python aaptOutput.py D://android/downloaded_apk/` 
After running you can see many txts in the folder `apkinfo`
* Open an `Android Emulator`(recommended), or connect an Android device to your computer
* Start autonomic test(Remember to add your apk absolute path):

    ```
    python startMonkey.py [apkDir]
    ```
After running you can check new `screenshot` folder

## TODO
Combine with `MonkeyRunner` or other test tools, to implement more powerful test.
