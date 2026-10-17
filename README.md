# FlashVideo Android (starter project)

FlashVideo is an Android WebView browser with a direct-media download button.

## Build an APK from a tablet using GitHub
1. Download and extract this ZIP.
2. Create a new GitHub repository named `FlashVideo`.
3. Upload the *contents* of this folder to the repository root (not the parent folder).
4. Open the repository's **Actions** tab and enable Actions if prompted.
5. Select **Build FlashVideo APK** and press **Run workflow**, or push to `main`.
6. Open the completed workflow run and download the `FlashVideo-debug-apk` artifact.
7. Extract the downloaded artifact ZIP and install `app-debug.apk` on your Android device. If prompted, allow installs from your browser/file manager.

## Important limitations
- This starter detects HTML5 video `currentSrc`, a `<source>` URL, or a few direct media links. It cannot reliably find every video.
- HLS/DASH streams, blob URLs, DRM, login-protected media, and sites that prohibit downloads may not work.
- Downloading is intended only for media you own or are authorized to save.
- This is a debug APK for testing. A release APK should be signed before public distribution.
- Vercel is not required to build this native Android APK. GitHub Actions builds it. Vercel can host a separate landing page if desired.
