# MyRadar Android SDK — Maven repository

Published releases of the MyRadar Android SDK, served from GitHub Pages at
`https://myradar.github.io/MyRadar-Android-SDK-Maven`.

```kotlin
// settings.gradle.kts
dependencyResolutionManagement {
    repositories {
        google()
        mavenCentral()
        maven { url = uri("https://myradar.github.io/MyRadar-Android-SDK-Maven") }
    }
}

// app/build.gradle.kts
dependencies {
    implementation("com.acmeaom.myradar:myradar-sdk:1.0.0")
}
```

Then call `MyRadarSdk.configure(apiKey = "<your key>")` once at launch. The SDK requires Android 10
(API 29) or later and a MyRadar API key.

A complete sample app is in [MyRadar-SDK-Samples](https://github.com/MyRadar/MyRadar-SDK-Samples)
under `android-demo/`.
