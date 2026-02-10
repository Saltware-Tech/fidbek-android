# Fidbek Android SDK

Binary Android SDK distribution.

## Version

`0.0.2`

## Install

In your top-level `settings.gradle` or `build.gradle` repositories:

```kotlin
maven("https://raw.githubusercontent.com/Saltware-Tech/fidbek-android/main/maven")
```

In app module:

```kotlin
implementation("com.fidbek:fidbek-android:0.0.2")
```

## Usage

```kotlin
Fidbek.initialize(
    application = this,
    token = "YOUR_TOKEN",
    baseUrl = "https://api.fidbek.dev"
)

// Optional manual trigger
Fidbek.open()
```

## Notes

- `0.0.2` includes missing transitive runtime dependency for `androidx.viewbinding.ViewBinding`.
- If you stay on `0.0.1`, add `implementation("androidx.databinding:viewbinding:8.13.2")` manually.
