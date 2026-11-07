# ISLAND REIGN — Android APK wrapper project

This project packages the supplied `ISLAND_REIGN_6.0_PHASE44.html` as a local
HTML game inside an Android WebView app. It preserves the HTML/JavaScript game
rather than rewriting it as a native C++ game.

## Build the APK using GitHub Actions (phone-friendly)

1. Create a new GitHub repository.
2. Upload the contents of this ZIP (not the ZIP file itself) to the repository.
3. Open the repository's **Actions** tab.
4. Select **Build ISLAND REIGN APK** and tap **Run workflow**.
5. When the run finishes with a green check, open it and download the
   `island-reign-debug-apk` artifact.
6. Extract the downloaded ZIP. It contains `app-debug.apk`.
7. Install the APK on your Android phone and test the game.

## Important

- This is a WebView APK wrapper, not a native C++ port.
- The app starts in landscape and uses immersive full-screen mode.
- The game uses WebGL/Three.js and localStorage. Actual graphics performance,
  touch behavior, save persistence, and Android WebView compatibility must be
  tested on the target phone.
- This build has not yet been compiled or tested on a physical Android device.
- The APK produced by this workflow is a debug APK. A release APK requires
  signing configuration before public distribution.
