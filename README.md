# Event Registration Mobile App Development with Java and Kotlin in Android Studio

Welcome to the Mobile App Development project! The Events Management App (EMA) is an Android application designed to streamline the organization and management of events. The app allows users to create, view, and manage event categories and events, ensuring a seamless experience for both event organizers and participants. Developed using Android Studio, the app leverages Java and Kotlin for its implementation, integrating modern UI elements and persistent data storage solutions.

## Introduction

This project aims to provide a comprehensive example of mobile app development in Android Studio, utilizing both Java and Kotlin. It serves as a learning resource for developers interested in exploring the differences and similarities between these two languages in the context of Android development.

## Installation

1. **Clone the repository**:
   ```
   git clone https://github.com/sarviin-hari/Event-Registration-Application-Android-Studio-.git
   ```
2. **Open the project in Android Studio**.
3. **Sync the project with Gradle files** to download all dependencies.
4. **Set up Firebase**:
   - Go to the [Firebase Console](https://console.firebase.google.com/) and create a new project.
   - Download the `google-services.json` file and place it in the `app` directory.
5. **Build and Run**:
   - Connect your Android device or start an emulator.
   - Click on the "Run" button in Android Studio.

#### Key Features
1. **User Authentication:**
   - **Sign Up/Registration:** Users can create an account by providing a username, password, and password confirmation. The registration details are stored securely using SharedPreferences.
   - **Login:** Users can log in with their credentials. The app verifies the entered username and password with the stored data and redirects successful logins to the Dashboard.

2. **Dashboard Activity:**
   - A central hub for accessing various functionalities, including the creation of new event categories and events.
   - Navigation drawer and toolbar with options to view all categories, add new categories, view all events, log out, refresh the dashboard, clear forms, and delete all categories/events.

3. **Event Category Management:**
   - **New Event Category:** Users can create new event categories by providing details like name, event count, and status. Each category is assigned a unique Category ID and can be saved to SharedPreferences.
   - **Category List:** A fragment displays all saved categories using a RecyclerView. The app supports viewing and managing categories.

4. **Event Management:**
   - **New Event:** Users can create new events, specifying details such as name, category ID, available tickets, and status. Each event is assigned a unique Event ID.
   - **Event List:** A fragment lists all saved events, displaying their details in a RecyclerView.

5. **Persistent Storage:**
   - The app uses SharedPreferences to store user credentials, categories, and events. It supports saving and restoring multiple entries using ArrayList and the GSON library.

6. **Advanced Features:**
   - **Google Maps Integration:** Displays the location of event categories on a map using the Geocoder API.
   - **WebView Integration:** Displays Google search results for events within the app, providing additional information to users.

#### Technology Used
- **Languages:** Java and Kotlin
- **Development Environment:** Android Studio
- **Data Storage:** SharedPreferences and / or Room Database 
- **UI Components:** RecyclerView, Fragments, Navigation Drawer, Toolbar, Floating Action Button (FAB)
- **APIs and Libraries:** GSON, Geocoder, Google Maps, WebView

#### Future Enhancements
- Implementing a comprehensive backend server for real-time data synchronization and user management.
- Enhancing the UI/UX with more interactive elements and responsive designs.
- Adding more advanced features such as event ticket booking, notifications, and user feedback mechanisms.

