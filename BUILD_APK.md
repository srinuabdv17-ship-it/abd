# Get the APK (about 5 minutes, free, no coding)

The app is a WebView wrapper around the same single-file app, so the APK and the web version are identical.

## Option A: GitHub (no installs needed)
1. Create a free account at github.com and make a new repository (private is fine).
2. Click "Add file" > "Upload files" and drag in EVERYTHING from this folder
   (including the hidden `.github` folder: unzip first, then drag the folder contents).
3. Open the "Actions" tab > "Build APK" > "Run workflow".
4. When it turns green, open the run, scroll to "Artifacts" and download `SSC-CGL-Maths-APK`.
5. Unzip it to get `app-debug.apk`, copy it to your phone and tap it.
   If asked, allow "Install unknown apps" for your file manager or browser.

## Option B: Android Studio
1. Open this folder in Android Studio (Koala or newer).
2. Let Gradle sync, then Build > Build Bundle(s) / APK(s) > Build APK(s).
3. The file is in app/build/outputs/apk/debug/app-debug.apk.

## Updating the content later
Replace `app/src/main/assets/index.html` with a new version of the app and build again.
Your best scores and the "already seen" question history are stored on the phone.
