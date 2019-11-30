This is a Readme how to build a simple ionic project for ios
1. add ionic platform ios "sudo ionic cordova platform add ios"
2. build "sudo ionic cordova build ios"
result -> worked fine!

How to add the Google Maps plugin to the APP
Add google maps plugin to project: $> sudo cordova plugin add cordova-plugin-googlemaps --variable API_KEY_FOR_IOS="AIzaSyAfugSygxEA3R9xOxfSYq9ZmQr6TLT__G4"
-> in my case it installed google maps with version 2.6.2 (sudo ionic cordova pluigin list)

AIzaSyAfugSygxEA3R9xOxfSYq9ZmQr6TLT__G4 -> api key for ios apps

sudo chmod -R 777 . setzt rechte aller dateien im ordner auf alles

set own variable in xcode (Add user defined settings)

PODS_PODFILE_DIR_PATH = ${SRCROOT}/.
PODS_ROOT = ${SRCROOT}/Pods

Question error 'GoogleMaps/GoogleMaps.h' file not found (maybe he dont find CocoaPods installation anymore??)

edit plugin/cordova-plugin-googlemaps/plugin.xml line 479  <pod name="GoogleMaps" spec="~> 3.1.0"/> to <pod name="GoogleMaps" spec="~> 2.7.0"/>

Code Snipet:
# googlemaps
