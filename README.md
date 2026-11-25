# GRAIN — Android camera prototype

A camera-first Android wrapper for the GRAIN retro camera web prototype. The app loads its bundled UI from Android's secure WebViewAssetLoader origin so browser camera APIs can be used with Android camera permission handling.

## Features in the bundled prototype
- Camera preview and switching (device/browser support permitting)
- Film-inspired live preview filters
- Capture/download photos
- Exposure, zoom, timer, aspect ratio, grid, filter strength, grain and white balance controls

## Build an APK with GitHub Actions
1. Create a GitHub repository and upload this project folder's contents.
2. Open the repository's **Actions** tab.
3. Select **Build GRAIN APK** and click **Run workflow** (or push to `main`).
4. When complete, open the workflow run and download the **GRAIN-debug-apk** artifact.
5. Extract the artifact ZIP on your Android phone, tap `app-debug.apk`, and allow installation from that source if Android asks.

The debug APK is unsigned for Play Store release but can be installed directly on a phone after allowing installation from the file manager/browser.

## Important prototype limitations
This is a first Android package prototype, not a fully native CameraX app. Camera/filter availability and some controls depend on Android WebView and device capabilities. Captured files are downloaded by the web layer; Gallery placement can vary by Android version. A later native CameraX/MediaStore build would provide more dependable gallery saving and deeper hardware controls.

Original film-inspired looks; not official Fujifilm simulations.
