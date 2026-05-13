#  Expo App

A cross-platform mobile application for Android and iOS built with Expo and React Native.

---

## Prerequisites

- [Node.js](https://nodejs.org) >= 18
- [Git](https://git-scm.com)
- Expo Go app on your device (optional, for quick previews)
- Android Studio (for Android emulator)
- Xcode (for iOS simulator, macOS only)

---

## Installation

### 1. Create the project

```bash
npx create-expo-app@latest
```

### 2. Navigate into the project

```bash
cd my-expo-app
```

### 3. Install dependencies

```bash
npm install
```

#### Lucide Icons

```bash
npx expo install lucide-react-native react-native-svg
```

#### Supabase

```bash
npx expo install @supabase/supabase-js @react-native-async-storage/async-storage
```

---

## Configuration

Create a `.env` file at the root of the project and add your Supabase credentials:

```env
EXPO_PUBLIC_SUPABASE_URL=https://your-project.supabase.co
EXPO_PUBLIC_SUPABASE_ANON_KEY=your-anon-key
```

---

## Running the App

### Start the development server

```bash
npx expo start
```

### Android

```bash
npx expo run:android
```

### iOS

```bash
npx expo run:ios
```

---

## Project Structure

```
app/
  _layout.tsx         # Root layout — global session context
  (tabs)/             # Bottom tab navigation
  auth/               # Authentication screens (login, register)
  contexts/           # React contexts
assets/               # Images, fonts, and static files
hooks/                # Custom React hooks
lib/                  # Utilities and Supabase client
```

---

## Tech Stack

- [Expo](https://expo.dev) — React Native framework
- [Expo Router](https://expo.github.io/router) — File-based routing
- [Supabase](https://supabase.com) — Auth and database
- [Lucide React Native](https://lucide.dev) — Icons

---

## Contributing

1. Fork the repository
2. Create a branch: `git checkout -b feature/my-feature`
3. Commit your changes: `git commit -m "Add my feature"`
4. Push to the branch: `git push origin feature/my-feature`
5. Open a pull request

---

