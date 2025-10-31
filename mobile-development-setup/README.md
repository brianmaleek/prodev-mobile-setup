# Expo Go Setup Documentation

## Objective

To set up **Expo Go** on a physical mobile device for testing and running React Native applications efficiently without relying on hardware emulators.

---

## Prerequisites

- Node.js LTS installed (`node -v` confirmed)
- Visual Studio Code (VS Code)
- macOS / Linux / Windows environment
- Stable internet connection

---

## Setup Steps

1. **Visited** [Expo Go Homepage](https://expo.dev/go)
2. **Selected** the latest SDK version
3. **Install** Expo Go on:
   - Android: via Google Play Store
   - iOS: via Apple App Store
4. **Open** the Expo Go app
5. **Create** a new Expo account (or log in)
6. **Link** physical device by scanning QR code generated from `npx expo start`

---

## Verification

After running:

```bash
npx create-expo-app my-first-app
cd my-first-app
npx expo start
```

I scanned the QR code from the terminal using the Expo Go app. The sample project loaded successfully on my phone, confirming the setup works correctly.

---

## Challenges Faced

- **Network latency:** The first connection took time because both devices were not on the same Wi-Fi.
- **Expo Go login loop:** Resolved by clearing cache and restarting the app.
- **Firewall blocking QR connection:** Fixed by allowing Node.js through the system firewall.

---

## Outcome

Expo Go is successfully installed and configured. The environment is ready for React Native mobile app development and live testing on a physical device.
