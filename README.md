# Workflow: Job Postings

A job posting app that favours both the job provider and the job seeker with competitive rates using a unique bidding system on job postings.
A Flutter application built with GetX for state management, featuring Google Sign-In authentication and local storage support.

## Features

- **Google Sign-In** — OAuth-based authentication via `google_sign_in`
- **GetX State Management** — Reactive state, dependency injection, and navigation using the `get` package
- **Persistent Local Storage** — User preferences and session data stored with `get_storage`
- **Cross-Platform** — Targets Android, iOS, and Web from a single codebase
- **Material Design UI** — Built with Flutter’s Material component library

## Tech Stack

|Layer           |Technology                                |
|----------------|------------------------------------------|
|Framework       |Flutter (Dart SDK `>=2.19.5 <3.0.0`)      |
|State Management|GetX (`get ^4.6.5`)                       |
|Local Storage   |GetStorage (`get_storage ^2.1.1`)         |
|Authentication  |Google Sign-In (`google_sign_in ^6.0.2`)  |
|Icons           |Cupertino Icons (`cupertino_icons ^1.0.2`)|

## Project Structure

```
workflow_flutter/
├── android/          # Android platform files
├── ios/              # iOS platform files
├── web/              # Web platform files
├── assets/
│   └── images/       # Image assets
├── lib/              # Dart source code
├── test/             # Unit and widget tests
├── pubspec.yaml      # Project dependencies
└── analysis_options.yaml
```

## Getting Started

### Prerequisites

- [Flutter SDK](https://docs.flutter.dev/get-started/install) installed and on your `PATH`
- Dart SDK `>=2.19.5 <3.0.0` (bundled with Flutter)
- Android Studio / Xcode for mobile targets, or a browser for web

### Installation

1. **Clone the repository**
   
   ```bash
   git clone https://github.com/lilshaji/workflow_flutter.git
   cd workflow_flutter
   ```
1. **Install dependencies**
   
   ```bash
   flutter pub get
   ```
1. **Configure Google Sign-In**
   
   Follow the [google_sign_in setup guide](https://pub.dev/packages/google_sign_in) to:
- Register your app in the [Google Cloud Console](https://console.cloud.google.com/)
- Download and place `google-services.json` (Android) or `GoogleService-Info.plist` (iOS) in the appropriate platform directories
1. **Run the app**
   
   ```bash
   # Android / iOS
   flutter run
   
   # Web
   flutter run -d chrome
   ```

### Build

```bash
# Android APK
flutter build apk --release

# iOS
flutter build ios --release

# Web
flutter build web
```

## Running Tests

```bash
flutter test
```

## Dependencies

|Package          |Version|Purpose                            |
|-----------------|-------|-----------------------------------|
|`get`            |^4.6.5 |State management, routing, DI      |
|`get_storage`    |^2.1.1 |Lightweight key-value local storage|
|`google_sign_in` |^6.0.2 |Google OAuth authentication        |
|`cupertino_icons`|^1.0.2 |iOS-style icon set                 |

## Contributing

1. Fork the repository
1. Create a feature branch (`git checkout -b feature/your-feature`)
1. Commit your changes (`git commit -m 'Add your feature'`)
1. Push to the branch (`git push origin feature/your-feature`)
1. Open a Pull Request

## Acknowledgements

Originally forked from [Neeraj-SD/workflow_flutter](https://github.com/Neeraj-SD/workflow_flutter).

## Resources

- [Flutter Documentation](https://docs.flutter.dev/)
- [GetX Documentation](https://pub.dev/packages/get)
- [GetStorage Documentation](https://pub.dev/packages/get_storage)
- [Google Sign-In for Flutter](https://pub.dev/packages/google_sign_in)
