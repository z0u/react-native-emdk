# react-native-emdk

This is a React Native bridge to Zebra's [EMDK] scanner library.

## Installation

```
npm install --save react-native-emdk
react-native link
```

If you have customised your build process, you may need to add the following to
your `MainApplication.java`:

```
import nl.kega.reactnativeemdk.ReactNativeEMDKPackage;
...
protected List<ReactPackage> getPackages() {
  return Arrays.<ReactPackage>asList(
      ...,
      new ReactNativeEMDKPackage()
      );
}
```

You will also need to download the EMDK .jar file from Zebra. For example,
grab the [EMDK SDK] and
copy `EMDK-A-0606065-MAC/SDK/addon-symbol_emdk-symbol-19/com.symbol.emdk.jar`
to `./node_modules/react-native-emdk/android/libs/com.symbol.emdk.jar`.

[EMDK]: http://techdocs.zebra.com/emdk-for-android/6-6/guide/about/
[EMDK SDK]: https://www.zebra.com/content/dam/zebra_new_ia/en-us/software/developer-tools/emdk-for-android/EMDK-A-0606065-MAC.zip
