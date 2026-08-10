# Chatter

A cross-platform real-time messaging app built with Flutter and Firebase. Users sign in, and messages sync live between devices.

## Features

- **Real-time messaging** — messages appear for the recipient as they're sent, without a refresh
- **User authentication** — sign-up and sign-in via Firebase Authentication
- **Persistent history** — conversations stored in Firebase and restored on login
- **Cross-platform** — a single Flutter codebase targeting Android and iOS

## Stack

- **Flutter** / Dart — UI and application logic
- **Firebase Authentication** — user sign-in
- **Cloud Firestore** — message storage and real-time sync

## Running locally

**Prerequisites:** Flutter SDK, and a Firebase project.

The Flutter project lives in the `chatter/` subdirectory, so run commands from there:

```bash
git clone https://github.com/pranay-kommuri/Simple-chatter-app.git
cd Simple-chatter-app/chatter
flutter pub get
```

Connect your own Firebase project using the FlutterFire CLI:

```bash
flutterfire configure
```

This generates `firebase_options.dart` and the platform config files. Then run:

```bash
flutter run
```

Firebase Authentication and Cloud Firestore both need to be enabled in the Firebase console.

## Project layout

```
chatter/
├── lib/            Dart source — screens, widgets, Firebase services
├── android/        Android platform config
├── ios/            iOS platform config
└── pubspec.yaml    Dependencies
```

## Roadmap

- Group conversations
- Media attachments
- Push notifications for messages received while the app is closed
