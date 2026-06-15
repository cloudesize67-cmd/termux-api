# Termux API — Claude Code Context

## Project Overview
This is an Android application (Termux API) that provides access to Android system
APIs from within the Termux terminal environment. It acts as a bridge between
Termux command-line tools and Android system features (camera, SMS, location, etc.).

## Tech Stack
- **Language**: Java / Kotlin
- **Build System**: Gradle (`build.gradle`, `gradlew`)
- **Target**: Android (APK)
- **Source**: `app/` directory

## Key Directories
- `app/` — Android app source (Java/Kotlin, resources, manifests)
- `gradle/` — Gradle wrapper files
- `.github/workflows/` — CI/CD workflows

## Development Guidelines
- Use `./gradlew build` to build the project
- Use `./gradlew test` to run unit tests
- Use `./gradlew assembleDebug` to build a debug APK
- Follow Android coding conventions
- Keep API permissions minimal — only request what's needed

## When Making Changes
1. Understand the existing Android API handler pattern before adding new features
2. Test on Android emulator or device when possible
3. Ensure the build passes (`./gradlew build`) before committing
4. Create PRs targeting the default branch
