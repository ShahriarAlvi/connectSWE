# ConnectSWE

## Overview

**ConnectSWE** is a Flutter-based mobile application designed to facilitate easy communication and appointment scheduling within a community. This app features user authentication, appointment management, and a user-friendly interface for managing posts and appointments.

## Features

- **User Authentication**: Simple login interface.
- **Home Screen**: Main dashboard for navigating the app.
- **Post Management**: View and manage posts.
- **Appointment Editor**: Create and edit appointments.

## Getting Started

### Prerequisites

- Flutter SDK: [Install Flutter](https://flutter.dev/docs/get-started/install)
- Dart SDK: Included with Flutter

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/ShahriarAlvi/connectSWE.git
    cd connectSWE
    ```

2. Install dependencies:
    ```bash
    flutter pub get
    ```

3. Run the app:
    ```bash
    flutter run
    ```

## Project Structure

```plaintext
lib/
├── common/
│   └── custom_button.dart
├── models/
│   └── post_model.dart
├── pages/
│   ├── home_page.dart
│   ├── login_page.dart
│   ├── post_screen.dart
│   ├── second_page.dart
│   └── appointment_editor.dart
├── services/
│   └── post_service.dart
└── main.dart
```

## Detailed Description

### main.dart

- **Function**: Initializes the app and sets the `LoginPage` as the home screen.
- **Widgets**: `MyApp`, `MaterialApp`.

### pages/login_page.dart

- **Function**: Displays a login button that navigates to `HomePage` upon clicking.
- **Widgets**: `LoginPage`, `Scaffold`, `AppBar`, `ElevatedButton`.

### pages/home_page.dart

- **Function**: Main screen after login. Provides navigation to `SecondPage`.
- **Widgets**: `HomePage`, `Scaffold`, `AppBar`, `ElevatedButton`.

### pages/second_page.dart

- **Function**: Displays a message indicating it's the second page.
- **Widgets**: `SecondPage`, `Scaffold`, `AppBar`, `Text`.

### pages/post_screen.dart

- **Function**: Displays a list of posts.
- **Widgets**: `PostScreen`, `Scaffold`, `AppBar`, `FutureBuilder`, `ListView`.

### pages/appointment_editor.dart

- **Function**: Form to edit and save appointment details.
- **Widgets**: `AppointmentEditor`, `Form`, `TextFormField`, `ElevatedButton`.

### models/post_model.dart

- **Function**: Defines the structure of a post.
- **Fields**: `id`, `title`, `content`, `date`.

### services/post_service.dart

- **Function**: Manages post data with methods to get, add, and delete posts.
- **Methods**: `getPosts`, `addPost`, `deletePost`.

### common/custom_button.dart

- **Function**: Reusable custom button widget.
- **Props**: `label`, `onPressed`.

## Running Tests

To run tests for the project, use the following command:
```bash
flutter test
```

Copy and paste the above Markdown code into your `README.md` file on GitHub, and it will format correctly when viewed on the repository page.
