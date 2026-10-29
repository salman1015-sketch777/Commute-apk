# Commute Tracker - Android APK Build Instructions

This Android Studio project was generated from your HTML code. It contains a complete native Android wrapper with WebView, hardware acceleration, and full offline persistence.

---

### Option 1: Build APK with Android Studio (GUI)
1. Download and open **Android Studio** (Koala / Hedgehog / Iguana or later).
2. Choose **File > Open...** and select this unzipped folder.
3. Wait for Gradle sync to complete.
4. Click **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
5. Once completed, a notification will appear: `APK(s) generated successfully: locate`.
6. Click **locate** to find your `app-debug.apk` file. You can transfer it directly to any Android phone and install!

---

### Option 2: Build APK via Command Line (Terminal / Mac / Linux / Windows)
Run from the root of this unzipped directory:

```bash
# On Linux / macOS:
./gradlew assembleDebug

# On Windows:
gradlew.bat assembleDebug
```

The generated APK will be at:
`app/build/outputs/apk/debug/app-debug.apk`

To install directly to a connected Android phone with USB debugging enabled:
```bash
./gradlew installDebug
```

---

### Option 3: Instant Build on Android Device using Termux
You can even build the APK directly on your Android phone using Termux:
```bash
pkg install openjdk-17 gradle
gradle assembleDebug
```

---

### Package Details:
- **Package Name**: `com.commutetracker.app`
- **Application Name**: `Commute Tracker`
- **Target SDK**: Android 14 / 15 (API 34)
- **Min SDK**: Android 6.0+ (API 23)
- **Offline HTML Location**: `app/src/main/assets/index.html`
