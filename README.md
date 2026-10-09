# 🥗 SnackTrack

**Your AI-powered nutrition companion.**

SnackTrack is a Flutter mobile application designed to help users understand their eating habits, track their nutrition, and build healthier routines. Using AI-powered meal analysis, the app provides estimated nutritional information, personalized food suggestions, and tools to support everyday wellness.

Developed as a software engineering graduation project.

## ✨ Features

* **🤖 AI-Powered Meal Analysis:** Describe a meal using text or voice and receive estimated nutritional information, including calories and macronutrients.
* **📊 Nutrition Dashboard:** View your daily nutrition and track your progress.
* **💧 Water Tracking:** Monitor your daily water intake.
* **📈 Weekly Reports:** Review nutrition trends and visualize your progress with charts.
* **💬 AI Nutrition Coach:** Get food-related guidance and suggestions through an AI-powered chat.
* **🍳 Recipe Generation:** Discover recipe ideas based on your preferences.
* **📅 Meal Planning:** Generate meal plans to help organize your eating habits.
* **⚖️ Weight Tracking:** Record and monitor changes in your weight.
* **👤 Profile and Settings:** Manage personal information and customize your experience.
* **♿ Accessibility:** Includes text scaling, high-contrast options, and reduced-motion support.
* **📱 Offline Support:** Uses local storage to keep supported information accessible offline and synchronize data with Firestore when connectivity returns.

## 🛠️ Tech Stack

| Technology                  | Purpose                           |
| --------------------------- | --------------------------------- |
| Flutter                     | Cross-platform mobile development |
| Dart                        | Application programming language  |
| Provider                    | State management                  |
| GoRouter                    | Navigation and routing            |
| Firebase Authentication     | User authentication               |
| Cloud Firestore             | Cloud database                    |
| Hive                        | Local data storage                |
| Google Gemini API           | AI-powered nutrition features     |
| FL Chart                    | Data visualization                |
| Flutter Local Notifications | Local notifications               |
| Firebase Cloud Messaging    | Push notifications                |

## 🏗️ Project Structure

The project uses a modular structure that separates screens, controllers, services, and data models.

```text
lib/
├── core/
├── models/
├── services/
├── controllers/
├── views/
├── app.dart
└── main.dart
```

* **Models:** Represent application data.
* **Services:** Handle external integrations, data access, and application services.
* **Controllers:** Manage application logic and state using `ChangeNotifier` and Provider.
* **Views:** Contain the user interface and screens.
* **Core:** Contains shared application components and utilities.

## 🧠 AI Integration

SnackTrack integrates the Google Gemini API to support nutrition-related features, including:

* Analyzing meal descriptions.
* Estimating nutritional values.
* Suggesting recipes and meal plans.
* Providing food-related guidance through an AI coach.

**Note:** AI-generated nutritional information is an estimate and may not be medically accurate. It should not replace professional dietary or medical advice.

## 🚀 Getting Started

Follow these steps to run SnackTrack locally.

### Prerequisites

Make sure you have the following installed:

* [Flutter SDK](https://docs.flutter.dev/get-started/install)
* [Dart SDK](https://dart.dev/get-dart)
* [Android Studio](https://developer.android.com/studio) or [Visual Studio Code](https://code.visualstudio.com/)
* A Firebase project
* A Google Gemini API key

### 1. Clone the Repository

```bash
git clone https://github.com/MohamedAbdAlmawjoud/SnackTrack.git
cd SnackTrack
```

### 2. Install Dependencies

```bash
flutter pub get
```

### 3. Configure Firebase

Configure Firebase for your Flutter project:

```bash
dart pub global activate flutterfire_cli
flutterfire configure
```

Select your Firebase project and the platforms you want to support.

In the Firebase Console:

1. Enable the authentication providers required by the application.
2. Set up Cloud Firestore.
3. Configure the appropriate Firestore security rules.
4. Configure any additional Firebase services used by the project.

### 4. Configure the Gemini API Key

Obtain an API key from [Google AI Studio](https://aistudio.google.com/).

If the application is configured to read the key from a Dart environment declaration, run:

```bash
flutter run --dart-define=GEMINI_API_KEY=YOUR_GEMINI_API_KEY
```

Replace `YOUR_GEMINI_API_KEY` with your actual key.

**Important:** The command above applies only if the application's code reads `GEMINI_API_KEY` through `String.fromEnvironment`. Check the implementation and existing configuration before running the project.

For production deployments, avoid exposing API keys in a client application. Consider routing AI requests through a secure backend.

### 5. Run the Application

Connect a device or start an emulator, then run:

```bash
flutter run
```

## 👥 Team Contributions

SnackTrack was developed collaboratively, with team members contributing to different parts of the application.

| Team Member   | Main Responsibilities                                                                          |
| ------------- | ---------------------------------------------------------------------------------------------- |
| Juwairia      | Authentication and onboarding                                                                  |
| Fatma         | Meal logging and AI meal analysis                                                              |
| Abdelrahman   | Dashboard and data visualization                                                               |
| Mohamed Tarek | Weekly reports and AI chat                                                                     |
| Mohamed Abd Almawjoud       | Profile and settings screens, local storage, Firestore security rules, and system architecture |

## 📚 What I Learned

Working on SnackTrack provided practical experience with:

* Building cross-platform applications using Flutter and Dart.
* Managing application state with Provider and `ChangeNotifier`.
* Integrating Firebase Authentication and Cloud Firestore.
* Working with local storage and offline functionality.
* Integrating AI-powered features through an external API.
* Creating reusable UI components and organizing application code.
* Implementing accessibility options.
* Collaborating on a team software engineering project.

## 🔮 Future Improvements

Potential improvements include:

* More personalized nutrition recommendations.
* Improved nutritional accuracy and user-adjustable meal estimates.
* Enhanced synchronization and offline conflict handling.
* Additional charts and nutrition insights.
* Stronger backend protection for AI API requests.
* More comprehensive automated testing.

## 📱 Project Status

SnackTrack is a collaborative graduation project built with Flutter, Firebase, and AI-powered features.

---

**SnackTrack: Make every meal count.** 🥑
