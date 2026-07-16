# Mapsted Sample App — Flutter

A Flutter sample application demonstrating how to integrate the **Mapsted Mobile SDK** (indoor
positioning, mapping, wayfinding, and location-based services) via the `mapsted_flutter` plugin.
Built against the current **Mapsted SDK 26.7.1** release.

A sample Mapsted licence file is included, providing access to the **Square One Shopping Centre**
(propertyId `504`) so you can run the app out of the box.

## Prerequisites

| | Minimum |
|---|---|
| Flutter | 3.x (stable) |
| Android `minSdkVersion` | **26** |
| iOS deployment target | **16.0** |
| JDK | 17 |

The sample consumes the `mapsted_flutter` plugin pinned to `v26.7.1` (see `pubspec.yaml`). Android
artifacts resolve from `https://mapstedhq.github.io/mapsted-android-maven`; iOS pods resolve from
`https://github.com/MapstedHQ/podspec.git`.

## Setup

1. Clone this repository:
   ```bash
   git clone https://github.com/MapstedHQ/MapstedSampleFlutter.git
   cd MapstedSampleFlutter
   ```
2. Fetch dependencies:
   ```bash
   flutter pub get
   ```
3. Ensure the Mapsted licence files are in place:
   - Android: `android/app/src/main/assets/demo_android_licence.key`
   - iOS: `ios/your_ios_license.key`

   The included sample licences cover Square One (propertyId `504`); use your own licence keys for
   your own properties.
4. Run on a connected device or emulator (Android API 26+ / iOS 16+):
   ```bash
   flutter run
   ```

## Documentation

Full integration guides, the Flutter getting-started tutorial, and API references are available at
[developer.mapsted.com/mobile-sdk](https://developer.mapsted.com/mobile-sdk/).

## Licence

This sample and the Mapsted Mobile SDK are distributed under the Mapsted proprietary licence — see
[`LICENSE`](LICENSE). All rights reserved.
