# Jo-Po SiteLog – Android project

A WebView wrapper around SiteLog.html (app/src/main/assets/index.html).
Supports GPS, camera/photo picker, "Save PDF" (Android print dialog) and CSV export to Downloads.

## Build the APK

**Option A – GitHub (no install needed)**
1. Create a new GitHub repository and upload everything in this folder (keep the .github folder).
2. Open the repo's Actions tab, run "Build APK" (it also runs on every push).
3. Download the `SiteLog-apk` artifact, unzip it, and install app-debug.apk on the phone (allow "install unknown apps").

**Option B – Android Studio**
Open this folder, wait for Gradle sync, then Build > Build APK(s).
The APK is in app/build/outputs/apk/debug/app-debug.apk.

**Command line** (JDK 17 + Android SDK installed): `./gradlew assembleDebug`

## Updating the app
Replace app/src/main/assets/index.html with the new SiteLog.html and rebuild.
Data is stored in the app's local storage on the phone, so keep the same package name when updating.
