# Expo Router Project Setup Documentation

## Objective

Set up the first mobile application using the **Expo Router template**.  
This includes documenting the scaffolding process, modifying the default screen, and understanding the effect of resetting the project.

---

## Project Setup Steps

### 1. Navigate to Project Directory

```bash
cd prodev-mobile-setup
```

Moved into the working directory where the Expo project would be initialized.

---

### 2. Initialize the Expo Project

```bash
npx create-expo-app@latest .
```

- Selected the **Expo Router** template when prompted.
- The CLI scaffolded the base project with the default directory structure:

```md
  app/
    (tabs)/
      index.tsx
      explore.tsx
    _layout.tsx
  assets/
  node_modules/
  package.json
  tsconfig.json
  app.json
```

- Installed dependencies automatically using npm.

---

### 3. Modify the Home Screen

Opened:

```bash
vi app/(tabs)/index.tsx
```

Located the default text:

```tsx
<Text>Welcome!</Text>
```

Changed it to:

```tsx
<Text>** First App Created **</Text>
```

saved the file.

This verified that the app could be customized successfully.

---

### 4. Run and Test the Application

Started the development server with:

```bash
npx expo start
```

Then:

- **For iOS:** Scanned the QR code using the iPhone Camera app.
- **For Android:** Scanned the QR code using the **Expo Go** app.

Result:  
The app launched on the physical device showing the modified home screen text:  
`** First App Created **`

---

### 5. Reset the Application

Executed:

```bash
npm run reset-project
```

#### Observation:

- The command **cleared the Metro bundler cache**.
- **Reinstalled dependencies** to ensure all packages matched the current configuration.
- **Deleted temporary build files**, restoring the project to a “clean state”.
- No user-created code (like the text edit) was removed, confirming the reset only affects caches and build artifacts.

---

## Outcome

The project was successfully created, modified, and tested.  
The `npm run reset-project` command proved useful for clearing build issues without deleting custom source files.

The environment is now fully ready for ongoing React Native development using Expo Router.
