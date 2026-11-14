# VR Investigation Management (Android WebView)

**Package:** `com.example.webviewapp`  
**Web app:** The supplied Google Apps Script deployment URL is configured in `MainActivity.java`.

## Build APK with GitHub Actions
1. Extract this ZIP file.
2. Create a new GitHub repository.
3. Upload the contents of this folder to the repository root (not the containing folder).
4. Open the repository's **Actions** tab.
5. Select **Build VR Investigation APK** and click **Run workflow** (or push to `main`).
6. Open the completed workflow run, then download the artifact named **VR-Investigation-Management-APK**.
7. Inside the downloaded artifact, install `app-debug.apk` on your Android phone.

## Build locally
Open the folder in Android Studio, allow Gradle sync, then run the `app` configuration or run:
`gradle assembleDebug`

## Notes
- Internet access, JavaScript, DOM storage, cookies and Google Apps Script redirects are enabled.
- The app supports HTML file chooser uploads and standard download links.
- The first launch requires an internet connection.
- This is a debug APK workflow; it is not a signed Play Store release.
- If your Apps Script deployment restricts access to authorized Google accounts, sign in through the page as required.
