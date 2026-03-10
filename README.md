# Fidbek Android SDK

Binary Android SDK distribution.

## Version

`0.3.0`

## Install

In your top-level `settings.gradle` or `build.gradle` repositories:

```kotlin
maven("https://raw.githubusercontent.com/Saltware-Tech/fidbek-android/main/maven")
```

In app module:

```kotlin
implementation("com.fidbek:fidbek-android:0.3.0")
```

## Usage

```kotlin
Fidbek.initialize(
    application = this,
    token = "YOUR_TOKEN"
)

// Optional manual trigger
Fidbek.open()

Fidbek.identify(
    userId = "user_123",
    email = "talha@example.com"
)

Fidbek.clearIdentity()
```

## Notes

- Core API is `initialize`, `open`, `identify`, `clearIdentity`, and `shutdown`.
- Flutter and React Native wrappers intentionally expose only this 5-method surface.
- Native attachment staging helpers remain available for compatibility but are deprecated.
- Fixed backend endpoint is internal: `https://api.fidbek.dev/v1/sdk/reports`.
- Current release line: `0.3.0`.
- Includes issue frequency selection, built-in localization for English, Turkish, Spanish, French, German, Portuguese, Arabic, Hindi, Japanese, and Simplified Chinese, plus English fallback for unsupported locales.
