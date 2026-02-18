# Fidbek Android SDK

Binary Android SDK distribution.

## Version

`0.1.5`

## Install

In your top-level `settings.gradle` or `build.gradle` repositories:

```kotlin
maven("https://raw.githubusercontent.com/Saltware-Tech/fidbek-android/main/maven")
```

In app module:

```kotlin
implementation("com.fidbek:fidbek-android:0.1.5")
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

- API is simplified in `0.1.x`.
- Fixed backend endpoint is now internal: `https://api.fidbek.dev/v1/sdk/reports`.
- `baseUrl`, `reportPath`, and `autoAttachScreenshot` are removed from public initialize API.
- Automatic screenshot capture on open flow is restored in `0.1.1`.
- Current release line: `0.1.5`.
