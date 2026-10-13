# 🎲 Cubik's — 3D Interactive Rubik's Cube & Solver

A sleek, modern, web-based 3D Rubik's Cube experience built with **Three.js** and **HTML5 Canvas**. Features smooth layer rotation physics, an interactive cosmic starfield backdrop, real-time timer and move tracking, solver playback, and a glassmorphism HUD interface.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Three.js](https://img.shields.io/badge/Three.js-r128-black?logo=three.js)](https://threejs.org/)
[![Vanilla JS](https://img.shields.io/badge/Vanilla-JS-yellow?logo=javascript)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

---

## ✨ Features

- **🎮 Intuitive Layer Manipulation**:
  - Drag directly on any cubie face to rotate the corresponding slice.
  - Tangent raycasting tracks drag velocity and seamlessly snaps layers into 90° increments with cubic easing.
- **🌌 Dynamic Cosmic Starfield**:
  - Custom canvas-based 3D star warp background that dynamically speeds up during automated shuffles and solves.
- **✨ Physical 3D Materials**:
  - Handcrafted beveled cubies using `MeshPhysicalMaterial` with clearcoat reflections, realistic ambient lighting, and dual directional rim lights.
- **⚡ Automated Solver & Undo**:
  - **Scramble**: Generates an animated 22-move random shuffle.
  - **Solve**: Plays back and animates the reverse solution sequence at dynamic speeds.
  - **Undo**: Reverses moves one by one.
  - **Reset**: Instantly reassembles the cube into solved state.
- **⏱️ Speedcubing Stats & LocalStorage**:
  - Live move counter and millisecond-accurate timer that starts on your first turn.
  - Automated state verification checking face normal alignment.
  - Victory modal displaying completion time and moves, preserving your **Personal Best** in `localStorage`.
- **📱 Fully Responsive & Zero Build**:
  - Self-contained in a single lightweight `index.html` file with zero build tools or dependencies required.
  - Touch-friendly controls with safe-area insets for mobile and tablet screens.

---

## 🕹️ Controls

| Action | Control |
|---|---|
| **Turn Face / Layer** | Click / Touch and drag across any cube face |
| **Orbit Camera** | Click / Touch and drag empty background space |
| **Zoom In / Out** | Mouse wheel scroll / Pinch |
| **Scramble** | Click **Scramble** button in dock |
| **Auto Solve** | Click **Solve** button in dock |
| **Undo Move** | Click **Undo** button in dock |
| **Reset Cube** | Click **Reset** button in dock |

---

## 🚀 Getting Started

Since Cubik's is completely self-contained with no package manager or build pipeline required, you can run it directly:

### 1. Clone the repository
```bash
git clone https://github.com/ayoubanlouf/cubiks.git
cd cubiks
```

### 2. Run locally
Simply open `index.html` in any modern web browser:
- Double click `index.html` in your file explorer, OR
- Serve with any local HTTP server:
  ```bash
  # Using Python
  python -m http.server 8000

  # Or using Node / npx
  npx serve .
  ```

Visit `http://localhost:8000` (or `http://localhost:3000`) in your browser.

---

## 🛠️ Built With

- **[Three.js (r128)](https://threejs.org/)** — WebGL 3D scene rendering, cameras, geometry, and materials
- **[HTML5 Canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)** — Warp star background animation
- **[Space Grotesk](https://fonts.google.com/specimen/Space+Grotesk)** — Modern typography
- **Vanilla CSS3** — Glassmorphic styling and responsive UI

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
