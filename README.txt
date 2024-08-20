README

# Readme.txt

## Phonics Application for Preschooler (FYPAPP)

### Table of Contents
1. Introduction
2. System Requirements
3. Installation and Setup
4. Running the System
5. Linking the System Components
6. Working with the Prototype
7. Database Setup and Management
8. Raw Data Management
9. Troubleshooting
10. Contact Information

---

### 1. Introduction
This project is an Android-based application designed as a learning material for teachers and students of preschooler. This document will guide you through the process of setting up, using, and managing the system, including its prototype, database, and raw data.

### 2. System Requirements
- Android Studio 4.1 or later
- Android SDK
- Java Development Kit (JDK) 8 or later
- Minimum API Level: Oreo
- Internet connection (for database setup and linking)


### 3. Installation and Setup
1. **Download the Project**: Download the zip file of the system.
   ```
2. **Open in Android Studio**: Open the project in Android Studio.
   - File -> Open -> Select the project folder.

3. **Sync the Project**: Allow Android Studio to sync the project with Gradle. This will download all necessary dependencies.

4. **Set Up the Emulator or Connect a Device**: Use an Android Emulator or connect an Android device to run the application.

### 4. Running the System
1. **Build the Project**: In Android Studio, go to Build -> Make Project or press `Ctrl+F9`.
2. **Run the Application**: Click the Run button or press `Shift+F10` to install and run the app on your selected device.

### 5. Linking the System Components
1. **Link Activities**: Ensure that each ImageButton in the MainActivity is linked to the appropriate activity in the Java code.
   - Use `Intent` in your Java code to navigate between activities.
   - Example:
     ```java
     Intent intent = new Intent(MainActivity.this, TargetActivity.class);
     startActivity(intent);
     ```

2. **Database Linking**: If your system uses a database, ensure that the database connection is properly configured.
   - Set up your Firebase/SQLite database as per instructions in the Database Setup section.

### 6. Working with the Prototype
1. **Prototype Setup**: Place all prototype resources (images, audio files, etc.) in the `res` folder.
2. **Resource Linking**: Ensure all resources are correctly linked in your XML and Java files.
   - Example: Link audio files to buttons using the `MediaPlayer` class in Java.

3. **Testing the Prototype**: Run the prototype in the emulator or on a physical device to ensure everything is functioning correctly.

### 7. Database Setup and Management
1. **Firebase Setup**:
   - Go to [Firebase Console](https://console.firebase.google.com/), create a new project, and add your Android app.
   - Download the `google-services.json` file and place it in the `app` directory.


3. **Data Insertion and Retrieval**: Implement methods for data insertion, retrieval, and deletion in your `DatabaseHelper` class.

### 8. Raw Data Management
1. **Storage Location**: Place all raw data files (like audio, images) in the appropriate folders inside the `res` directory.
   - Audio files: `res/raw/`
   - Images: `res/drawable/`

2. **Accessing Raw Data**: Use `R.raw.filename` or `R.drawable.filename` in your Java code to access these files.

### 9. Troubleshooting
- **No Action on Button Click**: Ensure that `onClick` listeners are properly set up in the Java code.
- **Resource Not Found**: Double-check the file paths and ensure that all resources are correctly placed in the `res` directory.
- **App Crash**: Check the Logcat in Android Studio for any error messages and resolve them as needed.

### 10. Contact Information
For any issues or questions, please contact:

- **Project Lead**: [AMIRAH NUR QISTINA]
- **Email**: [2021862694@student.uitm.edu.my]
- **Phone**: [0102077110]

---

End of Readme.txt

---
