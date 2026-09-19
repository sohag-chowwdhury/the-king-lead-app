# The King Lead Follow-up

Flutter Android app using Firebase Authentication and Cloud Firestore realtime streams.

## Firebase console prerequisites

1. Enable Authentication > Email/Password.
2. Create a Cloud Firestore database.
3. Deploy the included `firestore.rules`.

## Build

Run `flutter create --platforms=android --org com --project-name the_king_lead_app .` once inside this folder if generated Android scaffolding is absent. Keep `android/app/google-services.json`, then ensure the Google Services Gradle plugin is enabled. Run `flutter pub get` and `flutter build apk --release`.

Package name must remain `com.theking`.

The included GitHub Actions workflow can generate the release APK without a
local Flutter installation. Push this folder as the root of a GitHub repository,
open Actions > Build Android APK, and download the generated artifact.
