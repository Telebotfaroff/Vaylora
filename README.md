# Vaylora

**Entertainment without boundaries.**

Vaylora is a premium, cross-platform media discovery and playback app built with React Native and Expo. This repository is the independent Vaylora application codebase.

## Brand

- App name: **Vaylora**
- Android application ID: `com.vaylora.player`
- Deep-link scheme: `vaylora://`
- Visual identity: Midnight Black `#090E1B`, Electric Blue `#168BFF`, Ice Blue `#50C8FF`

## Features

- Stream and download media from configured providers
- Google Cast and DLNA support
- Watchlist and local media playback
- External player and downloader support
- Desktop synchronization
- Custom provider/plugin support
- Android TV support

## Development

### Requirements

- Node.js 18 or newer
- Android Studio and Android SDK for Android builds
- Expo CLI through the project dependencies

### Setup

```bash
git clone https://github.com/Telebotfaroff/Vaylora.git
cd Vaylora
npm install
npm run build:sandbox
```

### Run on Android

```bash
npm run android
```

### Android TV

```bash
npm run android:tv
```

### Tests and lint

```bash
npm test
npm run lint
```

## EAS builds

Vaylora must use its own Expo Application Services project and signing credentials. Do not reuse Vega's EAS project ID, Play Store service account, or signing keys.

After configuring the Vaylora EAS project and Android credentials:

```bash
npx eas-cli init
npx eas-cli build --platform android --profile preview
```

Store signing credentials and service-account files outside version control. Configure Play Store submission only after the Vaylora Play Console app and service account are ready.

## Project identity

This is an independent rebrand and application repository. The app's provider, playback, download, casting, and Android TV functionality is intended to remain intact while Vaylora-specific identity and release infrastructure are introduced.

## License and notices

See [LICENSE](./LICENSE) and [NOTICE](./NOTICE) for applicable license and attribution information.
