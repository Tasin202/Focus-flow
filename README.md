# FocusFlow – Android app

## Easiest: build the APK on GitHub (no Android Studio needed)
1. Create a new GitHub repo and upload everything in this folder (keep the `.github` folder).
2. Open the repo's **Actions** tab -> "Build Android APK" -> it runs automatically (or press **Run workflow**).
3. When it's green (~5 min), open the run and download **FocusFlow-APK** -> unzip -> `app-debug.apk`.
4. Send the APK to your phone, tap it, allow "install unknown apps", done.

## Or build locally (needs Node 20, JDK 17, Android Studio)
    npm install
    npx cap add android
    npx cap sync android
    npx cap open android      # then Build > Build APK(s)

The whole app lives in `index.html` (the build copies it into `www/`). After editing it, run `npx cap sync android` and rebuild.
