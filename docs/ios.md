### dart 
- [class constructors](https://www.dartlang.org/guides/language/language-tour#using-constructors)

### flutter
```bash
flutter create -i swift my-app
# change PRODUCT_BUNDLE_IDENTIFIER
# DEVELOPMENT_TEAM = MK6YZLR2TP
nvim ios/Runner.xcodeproj/project.pbxproj
flutter run
```
- check 設定->一般->プロファイルとデバイス管理->デベロッパAPP

### flutter plugin
- flutter create --template=plugin -i swift -a kotlin hello
- [document](https://flutter.io/developing-packages/)

### carthage
- brew install carthage
```
cat Cartfile
github "Alamofire/Alamofire"
github "SwiftyJSON/SwiftyJSON"
```
- carthage update --platform iOS
- 「Linked Frameworks and Library」=> add(+) button

/usr/bin/env xcrun xcodebuild -configuration Release VERBOSE_SCRIPT_LOGGING=YES -workspace Runner.xcworkspace -scheme Runner BUILD_DIR=/Users/developer/flwork/niuz/build/ios -sdk iphoneos -arch arm64 CODE_SIGNING_ALLOWED=NO CODE_SIGNING_REQUIRED=NO CODE_SIGNING_IDENTITY=""
