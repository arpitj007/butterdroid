# ButterDroid 🧈

A new open-source UI for stock Android — designed to be **smooth as butter**.

ButterDroid is built with modern, native Android technologies so the experience
stays fluid, lightweight, and true to the stock-Android look and feel.

## Tech stack

- **Language:** [Kotlin](https://kotlinlang.org/)
- **UI toolkit:** [Jetpack Compose](https://developer.android.com/jetpack/compose) with **Material 3**
- **Dynamic color:** Material You (Android 12+) for a native, theme-aware UI
- **Build system:** Gradle (Kotlin DSL) with a version catalog (`gradle/libs.versions.toml`)
- **Min SDK:** 24 (Android 7.0) · **Target/Compile SDK:** 35 (Android 15)

## Project structure

```
butterdroid/
├── app/                          # Application module
│   ├── build.gradle.kts
│   └── src/main/
│       ├── AndroidManifest.xml
│       ├── java/com/butterdroid/app/
│       │   ├── MainActivity.kt   # Compose entry point
│       │   └── ui/theme/         # Color, Theme, Typography
│       └── res/                  # Resources (strings, themes, icons)
├── build.gradle.kts              # Root build config
├── settings.gradle.kts
└── gradle/libs.versions.toml     # Centralized dependency versions
```

## Getting started

### Prerequisites

- [Android Studio](https://developer.android.com/studio) (latest stable) **or** the Android SDK + JDK 17+
- An Android device or emulator running API 24+

### Build & run

```bash
# Build a debug APK
./gradlew assembleDebug

# Install on a connected device/emulator
./gradlew installDebug
```

Or simply open the project in Android Studio and hit **Run** ▶.

> **Note:** Building requires the Android SDK. Set `sdk.dir` in a `local.properties`
> file (Android Studio does this automatically) or export `ANDROID_HOME`.

## Contributing

Contributions are welcome! This is an early-stage project, so there's lots to do.
Please open an issue to discuss significant changes before submitting a PR.

## License

ButterDroid is released under the [Apache License 2.0](LICENSE).
