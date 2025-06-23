# NavKit - A Modern Android GitHub Browser

NavKit is a feature-rich Android application that demonstrates best practices in modern Android development. It enables users to effortlessly explore GitHub profiles and repositories while leveraging the latest technologies like Jetpack Compose and Kotlin Coroutines. This project serves both as a useful tool and an educational resource for developers who want to learn about clean architecture, unidirectional data flow (MVI), and dependency injection using Koin.

## Table of Contents
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Architecture](#architecture)
- [Installation & Setup](#installation--setup)
- [Usage](#usage)
- [API Integration](#api-integration)


## Features
- **GitHub User Browsing**: Explore and search GitHub users seamlessly.
- **User Details**: View rich user profiles with comprehensive details.
- **Repository Exploration**: Browse a user’s GitHub repositories with ease.
- **Intuitive UI**: Built with Jetpack Compose for smooth, dynamic interfaces.
- **Robust Navigation**: Clean navigation architecture supported by Navigation Compose.
- **Resilient Error Handling**: Offline and error states handled gracefully.
- **State Management**: Managed through the MVI pattern ensuring a predictable UI.
- **Feedback System**: Real-time notifications and Snackbar alerts.

## Tech Stack

### Core Technologies
- **Kotlin**: Primary programming language for robust Android development.
- **Jetpack Compose**: Declarative UI toolkit for building native Android interfaces.
- **Kotlin Coroutines & Flow**: For efficient asynchronous operations and reactive programming.
- **Material Design**: Implements material design principles for a polished user experience.

### Key Libraries & Frameworks
- **Retrofit & OkHttp**: For RESTful API communication with GitHub.
- **Gson**: JSON serialization/deserialization.
- **Coil**: Lightweight image loading library for Compose.
- **Navigation Compose**: For handling in-app navigation.
- **Koin**: Dependency injection framework to manage application modules.
  
### Testing Tools
- **JUnit & Robolectric**: For unit testing, including UI and logic tests.
- **MockWebServer & Mockk**: For mocking network responses and dependencies.
- **Coroutines Test**: Facilitates testing asynchronous code effectively.
- **Koin Test**: Simplifies dependency injection testing.

## Architecture
NavKit is designed following the principles of Clean Architecture and utilizes the MVI (Model-View-Intent) pattern:
- **Clean Architecture**: Layers are clearly separated to ensure scalable and maintainable code.
- **MVI Pattern**: Promotes unidirectional data flow for predictable state management.
- **Repository Pattern**: Abstracts data sources and business logic from UI components.
- **Dependency Injection with Koin**: Streamlines the management of dependencies across the application.

## Installation & Setup

### Prerequisites
- Android Studio Bumblebee or later.
- Android SDK 33+
- An internet connection for fetching GitHub data.

### Steps
1. **Clone the Repository**
    ```bash
    git clone https://github.com/Rudra1502/NavKit.git
    ```
2. **Open Project in Android Studio**
    - Launch Android Studio and choose **Open an Existing Project**. Navigate to the cloned repository.
3. **Build the Project**
    - Allow Gradle to sync and download required dependencies.
4. **Run the App**
    - Connect an Android device or use an emulator, then click **Run** to launch the app.

## Usage
Upon launching NavKit, you will be presented with a user-friendly interface where you can:
- **Browse Users**: Navigate through a list of GitHub users.
- **View Details**: Tap on a user to see detailed information and repositories.
- **Navigate Seamlessly**: Enjoy smooth transitions between different screens with responsive UI feedback.

## API Integration
NavKit leverages the GitHub API to retrieve live data:
- **Users Endpoint**: Retrieve a list of GitHub users.
- **User Details Endpoint**: Get detailed profile information.
- **Repositories Endpoint**: List repositories by user.

**Base URL**: `https://api.github.com/`
