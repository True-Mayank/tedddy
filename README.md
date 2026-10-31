# LUXE Music

Offline Android music player using a WebView UI and Android Storage Access Framework.

## Features
- Select one local music folder; subfolders are ignored.
- Real embedded MP3 album artwork thumbnails.
- Artwork is extracted natively on Android and sent to the LUXE UI in the background.
- Browser fallback includes a small ID3v2 APIC artwork reader for MP3 files.
- List/grid views.
- Sort menu: title A-Z/Z-A, newest/oldest added, recently played, most played.
- Local favorites, recent songs and playlists.
- Native folder persistence.
- Native foreground playback service foundation.

## GitHub build
Upload this complete project to GitHub and build the `app` module with Android Studio/Gradle.


## UI update
This version uses one Library screen with four category tiles (Tracks, Playlist, Favourite, Recent), a persistent search field, and LUXE Music as the heading. The three-line options menu contains View, Sort Order, and Playing Order. Playlist detail screens have their own search and saved view/sort/playing-order preferences.


## UI and playback fixes in this build
- Browser playback uses the selected local audio files; Android playback sends the queue to the native foreground media service.
- The three-line menu opens the View, Sort Order, and Playing Order options.
- Playlist cards open an individual playlist screen with search, independent view/sort/playing order, add-song selection, play, and remove-from-playlist controls. Removing a song from a playlist does not remove it from the library.
- Customise LUXE opens appearance settings for accent theme, font, preset background, and an image background.
- JavaScript syntax was checked. Please test playback on your device/browser; actual audio format support depends on the platform decoder.


## Feature pack
- **Rename Song** and **Delete Song from Folder**: ⋮ on a song row, or "More" on the player. On Android the real file is changed; Android asks once for edit access to the music folder.
- **Slow + Reverb** (player): speed + pitch, reverb amount and room size, built-in and custom presets, optional per-song settings.
- **Playback Speed** (player): tempo only, pitch unchanged, optional per-song.
- **Crossfade**, **Gesture control**, **Dynamic album artwork colors**, **Find duplicate songs**: Customize LUXE → Playback & Library.
- **Full-Screen Visualizer** (player): Bars / Wave / Circle. Android asks for the microphone-style "record audio" permission only when it is opened; it is required by Android to read the audio spectrum.
- **Music Roulette**: 🎲 button next to Rescan on the Library screen.

The APK loads the files in `app/src/main/assets/`. Settings and presets are stored on the device.
