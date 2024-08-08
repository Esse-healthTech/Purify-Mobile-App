# Purify-Mobile-App



Purify is a comprehensive yoga-based mobile application designed to enhance your wellness journey. With Purify, users can seamlessly book yoga classes, purchase a wide range of wellness products, and access online classes from the comfort of their homes. The app provides a holistic approach to health and well-being, making it easier than ever to integrate yoga into your daily routine.

Key Features:

Class Booking: Easily find and book yoga classes at your convenience, with options for in-person sessions at various locations.
Online Classes: Access a variety of online yoga classes, allowing you to practice anytime, anywhere.
Product Purchases: Browse and buy a selection of wellness products, including yoga mats, clothing, accessories, and more.
Personalized Recommendations: Get class and product recommendations tailored to your preferences and goals.
User-Friendly Interface: Navigate the app effortlessly with its intuitive and user-friendly design.
Purify aims to provide a seamless and enriching experience for all users, whether you're a beginner or an experienced yogi.



-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

steps to install flutter 
-----------------------------------------------------------------
nstall Homebrew (if not already installed):
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

brew install flutter

flutter --version

flutter doctor

export PATH="$PATH:/opt/homebrew/bin"

------------------------------------------------------------------
for Windows 
-----------------------------------------------------------------
Installing Flutter on Windows


Visit the official Flutter SDK download page.

Extract the Flutter SDK:


Open the Start Search, type in "env," and select "Edit the system environment variables."
In the System Properties window, click on the "Environment Variables" button.
Under "System variables," find the Path entry, and click "Edit."
Add the full path to the flutter\bin directory (e.g., C:\flutter\bin) and click "OK" to save.

---------------------------------------------------------------------------------------------
state management :

Bloc using Clean Architecture : 
please follow the few tutorial for clean Architecture :
1: https://www.youtube.com/watch?v=KjE2IDphA_U&list=PLB6lc7nQ1n4iYGE_khpXRdJkJEp9WOech
2: https://www.youtube.com/watch?v=7V_P6dovixg

----------------------------------------------------------------------------------------------


basic structure of architecture 
----------------------------------------

lib/
├── core/
│   ├── themes/
│   │   ├── theme_controller.dart
│   │   ├── theme_data.dart
│   ├── localization/
│   │   ├── app_localizations.dart
│   │   ├── localization_controller.dart
├── data/
│   ├── repositories/
│   │   ├── auth_repository_impl.dart
│   ├── sources/
│   │   ├── remote/
│   │   │   ├── firebase_auth_source.dart
│   ├── models/
│       ├── user.dart
├── domain/
│   ├── repositories/
│   │   ├── auth_repository.dart
│   ├── usecases/
│   │   ├── send_otp_usecase.dart
│   │   ├── verify_otp_usecase.dart
├── presentation/
│   ├── blocs/
│   │   ├── auth_bloc/
│   │   │   ├── auth_bloc.dart
│   │   │   ├── auth_event.dart
│   │   │   ├── auth_state.dart
│   │   ├── theme_bloc/
│   │   │   ├── theme_bloc.dart
│   │   │   ├── theme_event.dart
│   │   │   ├── theme_state.dart
│   │   ├── localization_bloc/
│   │   │   ├── localization_bloc.dart
│   │   │   ├── localization_event.dart
│   │   │   ├── localization_state.dart
│   ├── screens/
│       ├── login_screen.dart
│       ├── home_screen.dart
├── main.dart

----------------------------------------------










