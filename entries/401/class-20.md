# Android Fundamentals

- Android apps can be written using Kotlin, Java, and C++ languages
- The Android SDK tools compile your code along with any data and resource files into an APK, an Android package, which is an archive file with an `.apk` suffix

> Each Android app lives in its own security sandbox, protected by the following Android security features

***The Android operating system is a multi-user Linux system in which each app is a different user***

### The Android system implements the principle of least privilege
- each app, by default, has access only to the components that it requires to do its work and no more

There are four different types of app components:
1. Activities
  - An activity is the entry point for interacting with the user
2. Services
  - A service is a general-purpose entry point for keeping an app running in the background for all kinds of reasons
3. Broadcast receivers
  - A broadcast receiver is a component that enables the system to deliver events to the app outside of a regular user flow, allowing the app to respond to system-wide broadcast announcements
4. Content providers
  - A content provider manages a shared set of app data that you can store in the file system, in a SQLite database, on the web, or on any other persistent storage location that your app can access

> Three of the four component types—activities, services, and broadcast receivers—are activated by an asynchronous message called an intent

#### The Manifest File

Before the Android system can start an app component, the system must know that the component exists by reading the app's manifest file, `AndroidManifest.xml`. Your app must declare all its components in this file, which must be at the root of the app project directory


