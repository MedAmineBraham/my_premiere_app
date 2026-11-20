# my_premiere_app

My first Flutter app: a small login-and-navigation demo with a green Material 3 theme and a French interface. It is a work in progress, built step by step while following a Flutter course (the anime page is planned for "TP 03").

## Features

- **Login screen**: email and password fields with a "Se connecter" button. There is no real authentication yet; the button shows a welcome message and goes straight to the home page.
- **Home page**: a simple welcome screen with a navigation drawer.
- **Navigation drawer**: avatar header, links to *Accueil* and *Animé*, and a *Déconnexion* (logout) action that returns to the login screen.
- **Anime page**: placeholder for now. The anime list is coming in a later step.

## Project structure

```
lib/
├── main.dart         # App entry point, theme (light green) and first route
├── login_page.dart   # Login form
├── home_page.dart    # Home screen with drawer
├── my_drawer.dart    # Side menu (navigation + logout)
└── anime_page.dart   # Placeholder for the anime list
assets/images/        # Images used by the app
```

## Getting started

### Prerequisites

- [Flutter SDK](https://docs.flutter.dev/get-started/install) (Dart `^3.13.5`)
- An Android emulator, iOS simulator, or a browser/desktop target

### Run the app

```bash
git clone https://github.com/MedAmineBraham/my_premiere_app.git
cd my_premiere_app
flutter pub get
flutter run
```

Platform folders for Android, iOS, web, Windows, macOS and Linux are included, so you can also run it with `flutter run -d chrome` or `flutter run -d windows`.

### Run the tests

```bash
flutter test
```

## Roadmap

- [ ] Build the anime list page
- [ ] Add form validation and hide the password text
- [ ] Add real authentication
- [ ] Replace the default package name (`com.example.my_premiere_app`) before publishing

## Tech

- Flutter / Dart
- Material 3 (`colorSchemeSeed: Colors.lightGreen`)
