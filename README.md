这是一个新的 [**React Native**](https://reactnative.dev) 项目，使用 [`@react-native-community/cli`](https://github.com/react-native-community/cli) 引导。

# 入门

> **注意**：请务必在继续之前完成 [设置您的环境](https://reactnative.dev/docs/set-up-your-environment) 指南。

## 步骤 1：启动 Metro

首先，您需要运行 **Metro**，这是 React Native 的 JavaScript 构建工具。

要启动 Metro 开发服务器，请在 React Native 项目的根目录中运行以下命令：

```sh
npm start
```

## 步骤 2：构建并运行您的应用程序

在 Metro 运行的情况下，从 React Native 项目的根目录打开一个新的终端窗口/窗格，并使用以下命令之一构建并运行您的 Android 或 iOS 应用程序：

### Android

```sh
npm run android # 首次17分钟
```

### iOS

对于 iOS，请记住安装 CocoaPods 依赖项（这只需在首次克隆或更新原生依赖项后运行）。


```sh
cd ios
# install CocoaPods dependencies
bundle install # 首次创建新项目时，运行 Ruby bundler 以安装 CocoaPods 本身：
bundle exec pod install # 每次更新原生依赖项
cd ..
npx react-native run-ios # npm run ios
# or
# open ios/MyApp.xcodeproj in Xcode or run `xeb -b ios`
# 点击 run 
```


## 生成 APK
```
cd android
./gradlew assembleRelease
```

## Gradle
```
# gradle.properties
org.gradle.java.home=/path/to/your/java/home 
```
```
# Environment Variable
$ export JAVA_HOME=/path/to/your/java/home
```

有关更多信息，请访问 [CocoaPods 入门指南](https://guides.cocoapods.org/using/getting-started.html)。

如果一切设置正确，您应该会在 Android 模拟器、iOS 模拟器或您连接的设备中看到您的新应用程序正在运行。

这是运行应用程序的一种方法 — 您也可以直接从 Android Studio 或 Xcode 构建它。

## 步骤 3：修改您的应用程序

现在您已经成功运行了应用程序，让我们进行更改！

在您选择的文本编辑器中打开 `App.tsx` 并进行一些更改。保存时，您的应用程序将自动更新并反映这些更改 — 这由 [Fast Refresh](https://reactnative.dev/docs/fast-refresh) 提供支持。

当您想强制重新加载时，例如重置应用程序的状态，您可以执行完全重新加载：

- **Android**：按两次 <kbd>R</kbd> 键或从 **开发菜单** 中选择 **“重新加载”**，通过 <kbd>Ctrl</kbd> + <kbd>M</kbd>（Windows/Linux）或 <kbd>Cmd ⌘</kbd> + <kbd>M</kbd>（macOS）访问。
- **iOS**：在 iOS 模拟器中按 <kbd>R</kbd>。

## 恭喜！:tada:

您已成功运行并修改了您的 React Native 应用程序。:partying_face:
