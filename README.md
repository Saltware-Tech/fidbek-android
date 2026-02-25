# Fidbek Android SDK

Binary Android SDK distribution.

## Version

`0.2.0`

## Install

In your top-level `settings.gradle` or `build.gradle` repositories:

```kotlin
maven("https://raw.githubusercontent.com/Saltware-Tech/fidbek-android/main/maven")
```

In app module:

```kotlin
implementation("com.fidbek:fidbek-android:0.2.0")
```

## Usage

```kotlin
Fidbek.initialize(
    application = this,
    token = "YOUR_TOKEN"
)

// Optional manual trigger
Fidbek.open()
```

## Notes

- API remains `initialize`, `open`, and `shutdown`.
- Fixed backend endpoint is internal: `https://api.fidbek.dev/v1/sdk/reports`.
- Current release line: `0.2.0`.
- Includes issue frequency selection, EN/TR localization (fallback EN), and reliability improvements from native source `0.2.0`.
