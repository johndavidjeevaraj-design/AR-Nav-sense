# AR-NavSense

**Sense the Path. Navigate the World.**

AR-NavSense is a Flutter-based Android accessibility and navigation project designed around voice-first interaction, location-aware navigation and emergency assistance workflows.

The project was developed as a team project. See the Team section below; individual contributions should be described separately and accurately when presenting this work in a personal portfolio.

## Project highlights

- Voice interaction using speech recognition and text-to-speech.
- GPS and map-based navigation interfaces using OpenStreetMap-related Flutter packages.
- Emergency SOS workflow and trusted-contact setup screens.
- Haptic feedback and accessibility-oriented display settings.
- Bluetooth device discovery interface.
- Camera access and an environment-awareness foundation.
- Multi-screen Flutter application with routing and reusable UI components.

**Implementation note:** A camera screen or AI-assistant interface does not by itself establish that production-grade object detection or a deployed AI model is present. Describe those capabilities as planned or foundational unless a working model and end-to-end behaviour have been verified on-device.

## Technology

- Flutter and Dart
- `go_router` for navigation
- `flutter_map` and `latlong2` for map UI
- `geolocator` for location access
- `speech_to_text` and `flutter_tts` for voice interaction
- `camera` for camera access
- `flutter_blue_plus` for Bluetooth integration
- Provider and SharedPreferences for state and local preferences
- Dio / HTTP for network requests

## Run locally

Requirements: Flutter SDK compatible with the Dart SDK constraint in `pubspec.yaml`, Android SDK and an Android device or emulator.

```bash
flutter pub get
flutter analyze
flutter test
flutter run
```

Build a debug APK:

```bash
flutter build apk --debug
```

The APK is generated under `build/app/outputs/flutter-apk/`.

## Accessibility and safety considerations

This is an academic/software project, not a certified assistive or emergency-response system. GPS accuracy, network availability, device permissions, speech recognition and SMS handling vary by device and environment. Users must not rely on the app as their sole emergency channel or as a replacement for established accessibility and emergency services.

Test all emergency flows with non-emergency contacts and explicit user consent. Do not send location or contact information without clear permission.

## Team

- Dharshan V
- JohnDavid J
- Lokesh V
- Byresh A

## Releases

Open the repository's [Releases](../../releases) page for available builds. Confirm the release tag and asset version before sharing a direct APK link.

## Project structure

```text
lib/
  constants/
  core/
  models/
  screens/
  services/
  theme/
  widgets/
android/
assets/
test/
```

## License

See [LICENSE](LICENSE) for the project license.
