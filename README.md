# Swap App Zone

![Flutter](https://img.shields.io/badge/Flutter-3.x%2B--025499?style=flat-square&logo=flutter&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-3.x%2B--0F74BD?style=flat-square&logo=dart&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)

A modern, cross-platform Flutter application for item swapping. Users can list items, request swaps, manage their profiles, and track swap history across iOS and Android. Built with Clean Architecture, Firebase, and a geo-location-aware feed.

---

## Screenshots

> Screenshots coming soon. Run the app locally to see it in action.

---

## Features

- Authentication: Secure user registration and login via Firebase Auth
- Home Feed: Browse and search items available for swap
- Geo-location Feed: Discover nearby swap offers based on your location
- Swap Requests: Send, receive, and manage swap requests
- In-app Messaging: Chat with other users about swap offers
- Profile Management: View and edit user profiles and swap history
- Real-time data sync via Firestore
- Responsive UI optimized for iOS and Android

---

## Tech Stack

| Category | Technology |
|----------|------------|
| Language | Dart (Flutter) |
| Architecture | Clean Architecture (Data / Domain / Presentation) |
| State Management | Provider |
| Backend | Firebase Auth, Firestore, Cloud Functions |
| Data Models | Freezed (immutable models) + Equatable |
| Serialization | json_serializable + build_runner |
| Location | Geo-location services |

---

## Architecture

This project follows Clean Architecture:

```
lib/
├── core/             # Shared utilities, routing, theme
├── features/
│   ├── auth/         # Login / registration
│   ├── feed/         # Home feed + search
│   ├── swap/         # Swap requests + history
│   ├── profile/      # User profile management
│   └── messaging/    # In-app chat
└── data/             # Firebase repositories & DTOs
```

---

## Getting Started

### Prerequisites

- Flutter 3.x+ installed ([Flutter install guide](https://docs.flutter.dev/get-started/install))
- A Firebase project (Android + iOS apps registered)

### Steps

1. Clone the repository
   ```bash
      git clone https://github.com/bavlymo1/Swap-App-Zone-.git
         cd Swap-App-Zone-
            ```

            2. Install dependencies
               ```bash
                  flutter pub get
                     ```

                     3. Configure Firebase
                        - Follow the [FlutterFire CLI guide](https://firebase.flutter.dev/overview)
                           - Run `flutterfire configure` to generate `firebase_options.dart`

                           4. Run code generation
                              ```bash
                                 flutter pub run build_runner build --delete-conflicting-outputs
                                    ```

                                    5. Run the app
                                       ```bash
                                          flutter run
                                             ```

                                             ---

                                             ## Contributing

                                             Contributions are welcome! Please open an issue or submit a Pull Request.

                                             ---

                                             ## License

                                             This project is open source for learning and demonstration purposes.

                                             ---

                                             Made by [Bahy Mohy](https://github.com/bavlymo1) | [LinkedIn](https://www.linkedin.com/in/bahy-mohy-0b5ab6407/)
