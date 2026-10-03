# FocusFlow

A calm, simple Pomodoro timer for Android.

## Features
- Focus, short break and long break sessions with a progress ring
- Skip, reset and quick +/- time buttons
- Task list with Pomodoros tracked per task
- Statistics: daily totals, streaks, 7-day chart, session history
- Custom durations, sounds, vibration, light/dark theme, 5 accent colors
- Works offline; all data stays on your device

## Download
Go to the **Actions** tab, open the latest successful run, and download
the **FocusFlow-APK** artifact. Unzip it and install `app-debug.apk`
on your phone (allow "install unknown apps" when asked).

## Build it yourself
Requirements: Node 20, JDK 17, Android Studio.

    npm install
    mkdir www && cp index.html www/
    npx cap add android
    npx cap sync android
    npx cap open android

Then in Android Studio: Build > Build APK(s).

## Project structure
- `index.html` – the entire app (HTML, CSS, JS)
- `capacitor.config.json` – Capacitor (Android wrapper) settings
- `package.json` – dependencies
- `.github/workflows/build-apk.yml` – builds the APK automatically

## License
MIT – see [LICENSE](LICENSE).
