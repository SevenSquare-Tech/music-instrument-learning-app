# 🎹 Music Instrument Learning App

**A React Native-based piano sampler for learning and playing music instruments with SoundFont support.**
Supports **SF2 (FluidSynth on Android)** and **SFZ (AudioKit on iOS)**.

[Build an Interactive Music Instrument Learning App in React Native](https://www.sevensquaretech.com/build-music-instrument-learning-app-react-native-code)

---

## 📖 Overview

The **Music Instrument Learning App** is a React Native library that brings a realistic piano learning experience to mobile apps.
It uses native audio processing for both iOS and Android platforms to produce high-quality sounds from SoundFont files.

---

## 🚀 Features

- 🎵 Load and play SoundFont files (`.sf2`, `.sfz`)
- 🎹 Interactive piano keyboard component
- 📱 Cross-platform support (iOS & Android)
- ⚡ Optimized performance for real-time playback
- 🧩 TypeScript support
- 🧰 Easy integration into existing React Native projects

---

## 📦 Installation

```bash
# Using npm
npm install music-instrument-learning-app

# Using yarn
yarn add music-instrument-learning-app
```

Then install iOS dependencies:

```bash
cd ios && pod install && cd ..
```

---

## 🧩 Usage Example

```tsx
import React from 'react';
import { View, StyleSheet } from 'react-native';
import { PianoSampler } from 'music-instrument-learning-app';

export default function App() {
  return (
    <View style={styles.container}>
      <PianoSampler
        soundFont="path/to/piano.sf2"
        octaves={2}
        onNotePress={(note) => console.log('Note pressed:', note)}
      />
    </View>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    justifyContent: 'center',
    alignItems: 'center',
  },
});
```

---

## ⚙️ Available Scripts

| Command | Description |
|----------|--------------|
| `yarn test` | Run Jest test cases |
| `yarn lint` | Run ESLint |
| `yarn typescript` | Run TypeScript type check |
| `yarn prepare` | Build the library using bob |
| `yarn release` | Publish a release with `release-it` |
| `yarn example` | Run the example project |
| `yarn bootstrap` | Setup dependencies for the library and example app |
| `yarn pods` | Install iOS pods |

---

## 📁 Project Structure

```
music-instrument-learning-app/
├── android/                     # Android native code (FluidSynth)
├── ios/                         # iOS native code (AudioKit)
├── cpp/                         # C++ audio processing bridge
├── src/                         # Main source code
├── lib/                         # Compiled output (Bob build)
├── example/                     # Example React Native app
├── react-native-piano-sampler.podspec
└── package.json
```

---

## 🧱 Development Setup

```bash
# Clone the repository
git clone https://github.com/SevenSquare-Tech/music-instrument-learning-app.git

# Navigate into the project
cd music-instrument-learning-app

# Install dependencies
yarn bootstrap

# Run example app
cd example && yarn ios
# or
cd example && yarn android
```

---

## 🧩 Peer Dependencies

Make sure you have these installed:

```json
{
  "react": "*",
  "react-native": "*"
}
```

---

## 🧪 Testing

```bash
yarn test
```

---

## 🧰 Linting and Formatting

```bash
yarn lint
```

Formatting is enforced using **Prettier** and **ESLint** rules configured in the project.

---

## 🐛 Issues & Contributions

Have a bug or feature request?
👉 [Open an issue](https://github.com/SevenSquare-Tech/music-instrument-learning-app/issues)
Pull requests are welcome!

---

## ⭐️ Support

If you find this library useful, please give it a **⭐️ star** on
[GitHub](https://github.com/SevenSquare-Tech/music-instrument-learning-app)!

---
