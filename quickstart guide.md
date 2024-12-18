# Dart
## quickstart guide
### abstract
This article will teach you how to 
+ get Dart SDK
+ setup the system environment setting
+ run a Dart project or `.dart` file in command prompt.
+ create a Dart project in command prompt.

### get Dart SDK
Before install Dart SDK, you have to check the [system requirements](https://dart.dev/get-dart#system-requirements)

Then, you have to [choose an installation option](https://dart.dev/get-dart#choose-an-installation-option).

Next, you can [Install the Dart SDK](https://dart.dev/get-dart#install).

After that, you have to set the system environment `PATH` and verify it.

#### [choose an installation option](https://dart.dev/get-dart#choose-an-installation-option)
To install and update the Dart SDK from the stable channel, choose one of the following options:

1. [Use a package manager](https://dart.dev/get-dart#install) (Recommended).
    
2. Use a [Dart Docker image](https://hub.docker.com/_/dart).
    
3. [Install Flutter](https://docs.flutter.dev/get-started/install).  
    If you've installed or plan to [install the Flutter SDK](https://docs.flutter.dev/get-started/install), it includes the full Dart SDK. The Flutter SDK includes the [`dart`](https://dart.dev/tools/dart-tool) CLI tool in Flutter's `bin` folder.
    
4. Download a ZIP archive from the [SDK Archive](https://dart.dev/get-dart/archive).
    
5. [Build the SDK from source](https://github.com/dart-lang/sdk/wiki/Building).

#### [Install the Dart SDK](https://dart.dev/get-dart#install)
> [!NOTE]
> I will only illustrate how to install the Dart SDK in Windows as my device is in Windows 11.

To install the Dart SDK in Windows 11, follow these steps.

1. [Install Chocolatey](https://semicolon.dev/windows/how-to-install-chocolatey-powershell).
2. Launch PowerShell with elevated permissions.
3. Change the current directory to `C:\`.
4. Type the following command in PowerShell.
   
```
choco install dart-sdk
```

#### set the system environment `PATH` (maybe optional)
1. find the location of Dart SDK (by default, it is located in `C:\tools\dart-sdk`
2. open system environment variable in Settings.
3. add that location to system environment `PATH`.

> [!TIP]
> By default, Chocolatey installs the SDK at `C:\tools\dart-sdk`.
> To change that location, set the [`ChocolateyToolsLocation`](https://stackoverflow.com/questions/19752533/how-do-i-set-chocolatey-to-install-applications-onto-another-drive/68314437#68314437) environment variable to your desired installation directory.

#### verify the Dart SDK
1. open command prompt.
2. type these following commands

```
dart --version
```

it should output like this

```
Dart SDK version: 3.2.4 (stable) (Thu Dec 21 19:13:53 2023 +0000) on "win_x64"
```

If it does not,

it indicates that the command prompt can not find Dart SDK.

The reason may be (but not limited to) as follows:

+ Dart SDK is not install on your device.'
+ The system environment `PATH` does not be set (or does not be set correctly).
+ You don't open new command prompt or restart it so that it does NOT make the change effect.
