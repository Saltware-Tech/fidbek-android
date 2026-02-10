# Fidbek Android SDK

Binary Android SDK distribution.

## Version

`0.0.1`

## Install

In your top-level `settings.gradle` or `build.gradle` repositories:

```kotlin
maven("https://raw.githubusercontent.com/Saltware-Tech/fidbek-android/main/maven")
```

In app module:

```kotlin
implementation("com.fidbek:fidbek-android:0.0.1")
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
