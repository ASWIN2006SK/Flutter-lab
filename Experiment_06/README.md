# Experiment 6: Data Persistence Using SQLite

## Aim
To design and develop a Flutter application that stores and retrieves student records using an SQLite database by implementing Create and Read operations.

## Description
Data persistence is the process of storing application data so that it remains available even after the application is closed or refreshed. SQLite is a lightweight relational database that stores information in tables. The sqflite package provides SQLite database operations in Flutter. Since this experiment is executed in Google Chrome, the sqflite_common_ffi_web package is used to enable SQLite support on the web platform.

The application is named StudentHub. It allows the user to enter a student's name, register number, department and email address. When the Save Student button is pressed, the application validates the entered details and inserts the record into the students table. The application then retrieves the saved records and displays them in the Student Records section.

The students table contains the following fields:
• id – INTEGER PRIMARY KEY AUTOINCREMENT
• name – TEXT NOT NULL
• registerNumber – TEXT NOT NULL
• department – TEXT NOT NULL
• email – TEXT NOT NULL

The main concepts used are DatabaseHelper for database initialization and operations, CREATE TABLE for creating the students table, INSERT for storing student details, SELECT for retrieving records, the Student model for converting data between objects and maps, and StatefulWidget with setState() for updating the interface.

The application was executed in Google Chrome at localhost:5555. The output screenshots show the student registration form and a saved student record displayed in the Student Records list.

## Project Structure
```
Experiment_06/
├── lib/
│   ├── main.dart
│   └── 
├── pubspec.yaml
└── README.md
```

## Running the Code
To run this experiment locally:
```bash
flutter pub get
flutter run -d chrome
```
