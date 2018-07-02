### flutter
```bash
flutter create -i swift my-app
# change PRODUCT_BUNDLE_IDENTIFIER
nvim ios/Runner.xcodeproj/project.pbxproj
flutter run
```
### carthage
- brew install carthage
```
cat Cartfile
github "Alamofire/Alamofire"
github "SwiftyJSON/SwiftyJSON"
```
- carthage update --platform iOS
- 「Linked Frameworks and Library」=> add(+) button
