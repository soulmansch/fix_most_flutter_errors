# fix_most_flutter_errors

These commands will solve many issues that you face when running a flutter app on an IOS device. It will also free some space by deleting the derived data in your xCode folder.

Make sure you are in the root of your Flutter project and paste the following code in your terminal:



flutter clean && <br>
rm -Rf ios/Pods && <br>
rm -Rf ios/.symlinks && <br>
rm -Rf ios/Flutter/Flutter.framework && <br>
rm -Rf Flutter/Flutter.podspec &&  <br>
rm ios/podfile.lock && <br>
cd ios && <br>
pod deintegrate && <br>
sudo rm -rf ~/Library/Developer/Xcode/DerivedData && <br>
flutter pub cache repair && <br>
flutter pub get && <br>
flutter pub upgrade && <br>
flutter pub upgrade --major-versions && <br>
Pod update && <br>
pod install && <br>
flutter run
