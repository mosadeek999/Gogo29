# Cadence

A local MP3 player for Android (Kotlin, Jetpack Compose, Media3 ExoPlayer). No account, ads, or network access;
the app does not request the INTERNET permission.

## Build

* **GitHub Actions:** push to GitHub (or run the workflow manually). `.github/workflows/build-apk.yml` builds
  `:app:assembleDebug` with JDK 17 and Gradle 8.7 and uploads `cadence-debug-apk` as an artifact.
* **Android Studio:** open this folder (Hedgehog or newer), let it sync, then Run.
* **Command line:** with Gradle 8.7 and the Android SDK (platform 34) installed: `gradle :app:assembleDebug`.

The Gradle wrapper jar is not included (it is a binary). If you want `./gradlew`, run `gradle wrapper --gradle-version 8.7` once.

## Versions
AGP 8.5.2, Kotlin 1.9.24, Compose compiler 1.5.14, Compose BOM 2024.06.00, Media3 1.3.1, compileSdk/targetSdk 34, minSdk 26.

## Status
This project was written without access to a Gradle/Android SDK toolchain, so it has **not been compiled or run**.
If the first build reports an error, it will be small and local; the first GitHub Actions run will show it.
