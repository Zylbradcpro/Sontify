# Sontify Android — Foundation 0.1.0

**Listen. Discover. Enjoy.**

This is a native Android project written in Kotlin with Jetpack Compose and AndroidX Media3.
It is not an Expo, Snack, Replit, or MIT App Inventor project.

## What is implemented

- Original Sontify black/white interface.
- Home, Search, Library, Friends, and Profile navigation.
- Android MediaStore scan for music files stored on the device.
- Real playback of those local audio files through AndroidX Media3.
- Play/pause and stop controls.
- Persistent mini-player while the app is open.
- Local playlist-name storage.
- Android audio permission handling.

## Important limitations (not disguised as completed features)

- This version plays audio files already stored on the user's phone. It does not yet stream an online catalog.
- Favorites are not yet connected to a complete interaction flow in this foundation.
- Playlists currently save names locally; adding/removing/reordering tracks is a next implementation step.
- Friends, cloud profiles, authentication, subscriptions, family accounts, artist uploads, royalties, advertising, and admin tools are not connected yet.
- The SQL file is a starter schema, not a deployed backend. A Supabase project, configuration, policies review, and server-side functions are required.
- No commercial music is bundled. Online streaming requires track-by-track rights or proper label/distributor/publisher agreements.
- The source has not been compiled or tested on a physical Android device in this environment.

## Build an APK using GitHub Actions

The repository includes `.github/workflows/android.yml`. After uploading this project to a GitHub repository:

1. Open the repository's **Actions** tab.
2. Select **Build Sontify Android APK**.
3. Run the workflow.
4. When it finishes, open the run and download the `sontify-debug-apk` artifact.
5. The APK is a debug build for testing, not a Play Store release.

A computer or a cloud build service is needed to compile this native Android project. GitHub Actions can run the build in the cloud, but uploading the source and downloading the artifact still requires account and browser steps.

## Local build requirements

- JDK 17
- Android SDK / Android Studio
- Android SDK Platform 35

Run:

```bash
gradle assembleDebug
```

The APK output is normally:

`app/build/outputs/apk/debug/app-debug.apk`

## Next development stages

1. Complete likes, track-based playlists, queue, seek controls, and background playback service.
2. Add Supabase authentication, profile sync, and secure backend configuration.
3. Add licensed online catalog ingestion and streaming.
4. Add artist verification, upload review, rights records, and artist analytics.
5. Add test-mode subscriptions, then production billing only after legal/business setup.
6. Add social, notifications, moderation, admin, and support systems.
7. Complete privacy/security review, device testing, and Play Store release preparation.
