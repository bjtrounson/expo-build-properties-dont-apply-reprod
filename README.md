# Welcome to this reproduction of this issue with expo-build-properties not applying with CNG

# To view the issue, follow these steps:
1. `npm install`
2. `npx expo prebuild`
3. Open the `android/build.gradle` file, you should see that the `ext` block that would normally load the values that expo-build-properties places in the `gradle.properties` file is missing.
4. To confirm that the expo-build-properties aren't loading you can build the app and it should still be using the minSdkVersion of 24 instead of 25 that is specified in the `expo-build-properties` plugin section.
