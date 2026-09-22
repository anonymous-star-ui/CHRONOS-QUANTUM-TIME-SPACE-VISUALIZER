# CHRONOS-QUANTUM-TIME-SPACE-VISUALIZER
A high-precision, interactive quantum chronometry dashboard and Progressive Web Application (PWA). Chronos bridges real-time civil timekeeping with fundamental quantum and relativistic definitions of time.

## 🚀 Live Demo & PWA Installation
Once hosted via GitHub Pages, this repository works as an offline-first **Progressive Web App (PWA)**. 
- Open the live link on mobile (Chrome / Safari / Edge).
- Tap **"Add to Home Screen"** or the browser install prompt to install it as a standalone app.

---

## 🔬 Core Visualizer Engines

### 1. 24-Hour Microsecond Precision Dial
- **True 24-Hour Radial Track:** Single rotation per solar day (00:00 to 23:59), eliminating AM/PM ambiguity.
- **Micro-Precision Sub-dials:** Real-time visual tracking down to milliseconds ($10^{-3}\text{ s}$) and microseconds ($10^{-6}\text{ s}$) using continuous high-resolution timestamps (`performance.now()`).
- **Timezone Detection:** Automatic localized timezone identification with instant switching between IST, UTC, EST, CST, and JST.

### 2. Cesium-133 Atomic Fountain Interior
- Visualizes the international SI definition of 1 second ($9,192,631,770$ radiation cycles).
- Simulates the laser cooling molasses, vertical atomic toss (fountain), Ramsey microwave cavity interrogation, and the quantum hyperfine transition ($F=3 \to F=4$).

### 3. Strontium-87 Optical Lattice Clock
- Simulates the next-generation optical lattice clock transition at $\approx 429\text{ THz}$.
- Displays the 813 nm magic-wavelength standing laser wave (egg-crate optical potential wells) holding atoms with zero Doppler shift while swept by a 698 nm crimson probe clock laser.

### 4. Relativistic Photon Engine
- Explores Einstein's relativistic relationship between space, distance, and the invariant speed of light ($c = 299,792,458\text{ m/s}$).
- Calculates transit durations ($\Delta t = \frac{d}{c}$) across planetary, astrophysical, and laboratory scales accompanied by an animated light-clock mechanism.

---

## 🛠️ Tech Stack
- **Frontend:** Vanilla JavaScript (ES6+), HTML5 Canvas, Modern CSS Glassmorphism
- **Precision:** `requestAnimationFrame`, `Intl.DateTimeFormat`, `performance.now()`
- **PWA:** Web App Manifest (`manifest.json`), Offline Cache Service Worker (`sw.js`)
- **Zero External Dependencies:** Completely lightweight, zero-npm, runs entirely in the browser.

---

## 📂 Project Structure
```text
├── index.html        # Unified application dashboard
├── manifest.json     # PWA configuration
├── sw.js             # Service Worker for offline PWA installation
├── LICENSE           # MIT License
└── README.md         # Project documentation
