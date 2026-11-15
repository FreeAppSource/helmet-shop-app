# Helmet Shop App

> 👨‍💻 Developed by **[Suresh Kumar Meesala](https://github.com/SureshKumarMeesala)** · 🎨 UI design by **Luka Dadiani** (credits below)

A mobile app built with **React Native (0.88+)**, **Expo SDK 58+** and **Expo Router**, using **JavaScript and JSX (`.js`, `.jsx`)**. Every screen is built from the original Sketch design `helmet-shop-app-concept-lukadadiani.sketch` by **Luka Dadiani**: one route per artboard, with the artboard's layout, colours, images and text.

![Helmet Shop App screens](./showcase.jpg)

## 📱 Screens (2 design artboards)

Listed in the order of the app's flow. "Taps" is the number of tap targets wired on the screen (buttons, tabs, back arrows, list rows).

| # | Screen (artboard) | Route | Size | Taps |
|---|---|---|---|---|
| 1 | **Home** · start screen | `src/app/home.jsx` | 463 × 948 | 1 |
| 2 | **Product** | `src/app/product.jsx` | 440 × 948 | 5 |

Screenshots of every screen are in [`screenshots/`](./screenshots).

## 🧩 How it's built

- `src/screens/*.json`: each design artboard converted to screen data (vector shapes, gradients, image fills, masks, shadows, blurs and rich text, positioned as in the design), plus its tap targets
- `src/sketch/SketchScreen.jsx`: draws a screen at the device's width with `react-native-svg`, native `Text`/`TextInput` and `expo-blur`, and handles navigation between screens
- `src/app/`: Expo Router routes, one per artboard (`index.jsx` opens the start screen)
- `assets/images/`: images used by the design

## 🛠️ Tech Stack

- **Framework**: React Native 0.88+ / Expo SDK 58+
- **Navigation**: Expo Router (file-based routing)
- **Language**: JavaScript & JSX (`.js`, `.jsx`)
- **Rendering**: `react-native-svg`, `expo-blur`
- **Fonts**: Google Fonts via `@expo-google-fonts` (Nunito Sans), standing in for the design's original fonts where those aren't free

<!-- run-locally:start -->

## ▶️ Run locally

```bash
npm install
npx expo start
```

Then press `i` for the iOS simulator, `a` for Android, or `w` for the web, or scan the QR code with Expo Go.

<!-- run-locally:end -->

<!-- developer:start -->

## 👨‍💻 Developer

This React Native app was developed by **Suresh Kumar Meesala**.

| | |
|---|---|
| Developer | [Suresh Kumar Meesala](https://github.com/SureshKumarMeesala) |
| GitHub | [@SureshKumarMeesala](https://github.com/SureshKumarMeesala) |
| Organization | [FreeAppSource](https://github.com/FreeAppSource) |
| Repository | <https://github.com/FreeAppSource/helmet-shop-app> |

<!-- developer:end -->

---

<!-- design-credits:start -->

## 🎨 Design Credits

This app is based on the free **Helmets App Shop Concept** design by **Luka Dadiani**, downloaded from Sketch App Sources. All visual design credit goes to the designer. The screens are reproduced from the original Sketch file; fonts that aren't free are replaced with similar Google Fonts, so some details may differ slightly from the original.

| | |
|---|---|
| Designer | [Luka Dadiani](https://www.sketchappsources.com/contributor/lukadadiani) |
| Original design | [Helmets App Shop Concept](https://dribbble.com/shots/11589763-DAY-02-Helmet-Shopping-App) |
| Downloaded from | [Sketch App Sources](https://www.sketchappsources.com/free-source/4433-helmets-app-shop-concept-sketch-freebie-resource.html) |
| Dribbble | <http://www.dribbble.com/lukadadiani> |
| Twitter | <https://twitter.com/lukadadiani> |
| Website | <https://www.linkedin.com/in/luka-dadiani-3293a915> |
| Original file | `helmet-shop-app-concept-lukadadiani.sketch` |
| License / usage | Not stated on the page. Free download; give credit (Sketch App Sources Terms). Confirm with the designer before commercial use. |

**Attribution:**

> UI design: "Helmets App Shop Concept" by Luka Dadiani (https://dribbble.com/shots/11589763-DAY-02-Helmet-Shopping-App), downloaded from Sketch App Sources (https://www.sketchappsources.com/free-source/4433-helmets-app-shop-concept-sketch-freebie-resource.html).

The original design source files are not included in this repository; get them from the links above. This app's **code** is released under the [MIT License](./LICENSE); the visual design remains the designer's (see [NOTICE](./NOTICE)).

Photos, brand logos and avatars inside the design may belong to third parties and are not covered by the designer's permission.

<!-- design-credits:end -->
