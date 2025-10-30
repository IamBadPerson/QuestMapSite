# 🗺️ QuestMap

**QuestMap** is a **fantasy-themed fitness tracker and progress mapper** built with **Expo React Native**. It transforms your **real-world movement** into **in-game travel** across iconic fictional worlds such as **the Sword Coast**, **Middle-earth**, and **Narnia**.

Every step you take contributes to your journey — walk to Waterdeep, trek across Mordor, or hike through Lantern Waste.

---

## ✨ Features

* **🌍 World Progression**
  Select a fantasy world and travel along legendary routes such as the Sword Coast or the Shire Road.

* **🚶 Step & Distance Tracking**
  Currently supports manual entry, with planned integration for **Google Fit** and **Apple Health** to automatically track real-world steps and distances.

* **📜 Route History**
  Save, view, and continue your progress with **persistent local storage** powered by AsyncStorage.

* **📈 Interactive Charts**
  Visualize your progress with **animated daily and cumulative charts**, tracking milestones and achievements.

* **📶 Offline Support**
  Once set up, the app works fully **offline**, keeping your adventure alive wherever you roam.

---

## 🛠️ Tech Stack

| Category    | Technology                                                                                               |
| ----------- | -------------------------------------------------------------------------------------------------------- |
| Framework   | [Expo React Native](https://expo.dev)                                                                    |
| Storage     | [@react-native-async-storage/async-storage](https://github.com/react-native-async-storage/async-storage) |
| Charts      | [react-native-gifted-charts](https://github.com/AbelTesfaye/react-native-gifted-charts)                  |
| Fitness API | [react-native-google-fit](https://github.com/StasDoskalenko/react-native-google-fit) *(planned)*         |

---

## ⚙️ Installation

### Clone the repository

```bash
git clone https://github.com/IamBadPerson/Questmap.git
cd Questmap
```

### Install dependencies

```bash
npm install
```

### Start the development server

```bash
npx expo start
```

> 💡 Tip: Running on a **physical device** gives more accurate step and distance tracking.

---

## 📦 Build for Android

To generate an APK:

```bash
npx expo build:android -t apk
```

Once the build completes, download the APK from the Expo dashboard and install it on your device.

---

## 🗂 Folder Structure

```
questmap/
├── assets/                  # Icons, JSON data (e.g., Sword Coast distances)
├── components/              # Reusable UI components
├── screens/                 # App screens and navigation
├── utils/                   # Helper functions (progress, formatting, etc.)
├── App.js                   # Main entry point
└── package.json             # Project metadata
```

---

## 🧭 Roadmap

Planned features and enhancements are tracked in **GitHub Issues**:
👉 [QuestMap Roadmap](https://github.com/IamBadPerson/Questmap/issues)

Highlights include:

* Integration with Google Fit and Apple Health
* Social progress sharing (“party travel” feature)
* New worlds (Tamriel, Thedas, and Faerûn expansion routes)
* Achievement badges and collectibles

---

## 🤝 Contributing

QuestMap follows a **GitFlow-based workflow**, with branches for `main`, `develop`, and feature branches.

1. **Fork** the repository or clone it directly.
2. Create a **feature branch** from `develop` using:

   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Make your changes and **commit** them with clear messages:

   ```bash
   git commit -m "Add new Sword Coast route data"
   ```
4. **Merge** into `develop` or open a **Pull Request** for review.
5. When ready for release, `develop` is merged into `main`.

> ⚙️ Default Expo and React Native structure is used to keep the project maintainable and familiar for contributors.

---

## 🧑‍💻 Development Workflow

Typical development cycle for QuestMap:

1. **Pull latest changes**

   ```bash
   git pull origin develop
   ```
2. **Create a feature branch** (GitFlow convention):

   ```bash
   git checkout -b feature/add-chart-animation
   ```
3. **Run locally** and test on Expo:

   ```bash
   npx expo start
   ```
4. **Debug & fix issues** using React Native DevTools or Expo logs.
5. **Commit changes** frequently with clear, scoped messages.
6. **Push** and open a pull request:

   ```bash
   git push origin feature/add-chart-animation
   ```
7. **Code review** and merge back into `develop`.

---

## 🧰 Common Development Commands

| Task                    | Command                                  | Description                                      |
| ----------------------- | ---------------------------------------- | ------------------------------------------------ |
| Start project           | `npx expo start`                         | Launch Expo Dev Tools in browser                 |
| Run on Android emulator | `npm run android`                        | Starts project in Android Studio emulator        |
| Run on iOS simulator    | `npm run ios`                            | Starts project in Xcode iOS simulator (Mac only) |
| Run on physical device  | Scan QR code                             | Use Expo Go app to preview on your phone         |
| Install dependency      | `npm install package-name`               | Adds a new package                               |
| Remove dependency       | `npm uninstall package-name`             | Removes a package                                |
| Clear cache             | `expo start -c`                          | Clears Metro bundler cache                       |
| Lint check              | `npm run lint`                           | Check code for formatting and syntax issues      |
| Build Android APK       | `npx expo build:android -t apk`          | Build an Android package                         |
| Build Android AAB       | `npx expo build:android -t app-bundle`   | Build an app bundle for Play Store               |
| EAS build               | `eas build -p android --profile preview` | Build using Expo Application Services            |

---

## 🧪 Testing & Debugging

* Use **Expo Go** on mobile for real-device testing.
* Enable **React Native Debugger** or Chrome DevTools for console and network inspection.
* Test data persistence using AsyncStorage test utilities.
* Verify UI consistency using Expo Preview across devices.
* Use `console.log` for in-code debugging; strip logs before production.

---

## 🧩 Code Style & Structure

* **Language:** JavaScript (ES6+)
* **Components:** Functional components using React Hooks (`useState`, `useEffect`).
* **State Management:** Local state; simple and component-scoped.
* **Styling:** React Native `StyleSheet.create()` or Tailwind (if added later).
* **Storage:** AsyncStorage with wrapper functions for safety.
* **Commit Messages:** Use short imperative messages (e.g., *Add*, *Fix*, *Refactor*).

---

## 📜 License

This project is licensed under the **MIT License**.
See the [LICENSE](LICENSE) file for full details.

---

## 🏰 Acknowledgements

* **Forgotten Realms Wiki** — for Sword Coast lore and route inspiration
* **Expo** and **React Native** communities — for exceptional tools and documentation
* **You**, the adventurer — for turning **steps into stories** and making fitness an epic quest

---

## 🧝‍♂️ Motto

> “Every journey begins with a single step — and some steps take you to new worlds.”
