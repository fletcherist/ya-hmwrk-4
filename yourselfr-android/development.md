Support to package apps for 64-bit devices, it's possible to specify 64-bit targets using the --xwalk64bit option in the build command:


cordova plugin add cordova-plugin-crosswalk-webview

cordova clean
cordova build android --xwalk64bit



x86 не работает на устройстве с x64 (ещё бы он работал)

Необходимо запускать отдельно билд x86 & x64

Разобрался с отладкой через Chroma Dev Tools

Apk скомпилировался для x64, но отказывается загружаться вьюха из-за «Uncaught TypeError: Cannot read property 'querySelector' of null»



