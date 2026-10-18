# ⚡ Neon Core — CrazyGames Edition

[![CrazyGames SDK v3](https://img.shields.io/badge/CrazyGames_SDK-v3.0-purple.svg)](https://docs.crazygames.com)
[![Three.js](https://img.shields.io/badge/Three.js-r128-black.svg)](https://threejs.org/)
[![Build Size](https://img.shields.io/badge/Build_Size-48_KB-00ffff.svg)](index.html)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

A high-speed, arcade 3D cyber-runner built specifically for the **CrazyGames** platform. Guide your glowing plasma core through dangerous neon sectors, dodge fatal red laser mines, collect cyan data fragments, and adapt to micro and heavy chassis power-ups.

---

## 🎮 Game Highlights

- **Standalone Single-File Architecture:** The entire game logic, 3D engine integration, styling, and sound synthesizer live inside a single, zero-dependency `index.html` file.
- **Cyberpunk Aesthetics:** Styled with Google Fonts (`Orbitron` & `Rajdhani`), neon bloom glows, and dynamic reactive lighting.
- **Synthesized Audio:** Custom procedural Web Audio API synthesizer for jumps, data pickup chirps, chassis shifts, and cybernetic alarms (no bulky external audio files).
- **Responsive Controls:** Full support for Desktop (WASD / Arrow Keys + Space) and Mobile touch screens (virtual D-pad + Jump button).
- **System Pause Menu:** Dedicated pause state mapped to `P` and `Escape`, halting the game loop cleanly.

---

## 🕹️ CrazyGames SDK v3 Integration

This edition is fully compliant with the latest **CrazyGames SDK v3** publisher guidelines:

| Feature | Implementation | Trigger |
| :--- | :--- | :--- |
| **SDK Initialization** | `window.CrazyGames.SDK.init()` | Runs on page load with fallback safeguards |
| **Gameplay Start** | `window.CrazyGames.SDK.game.gameplayStart()` | Starting a run, resuming from pause, or reviving |
| **Gameplay Stop** | `window.CrazyGames.SDK.game.gameplayStop()` | Pausing, Game Over, or Sector Secured |
| **Happytime** | `window.CrazyGames.SDK.game.happytime()` | Celebratory trigger when a sector is secured |
| **Rewarded Video Ad** | `window.CrazyGames.SDK.ad.requestAd('rewarded')` | Revive Core button on System Failure |
| **Midgame Interstitial** | `window.CrazyGames.SDK.ad.requestAd('midgame')` | Sector transitions (with 60-second UX cooldown) |
| **Banner Ad Container** | `window.CrazyGames.SDK.banner.requestBanner()` | Responsive 300x250 slot on Pause screen |

---

## 📁 Repository Structure

```
neon-core-crazygames/
│
├── index.html                    # Complete standalone single-file game
├── CRAZYGAMES_SUBMISSION_GUIDE.md # Step-by-step portal submission guide
│
├── build/
│   └── neon_core_crazygames_v2.zip # Ready-to-upload ZIP build (< 50 KB)
│
└── media/
    ├── covers/                   # Official CrazyGames cover artwork
    │   ├── cover_landscape_1920x1080.png  (16:9 Landscape)
    │   ├── cover_portrait_800x1200.png    (2:3 Portrait)
    │   └── cover_square_800x800.png       (1:1 Square)
    │
    ├── videos/                   # Gameplay preview trailers (< 20s, MP4)
    │   ├── preview_landscape_16x9.mp4
    │   └── preview_portrait_9x16.mp4
    │
    └── artwork/                  # High-resolution concept renders
        ├── Neon Cyberpunk Arcade Track.png
        ├── Neon Cyberpunk Wireframe Runner.png
        └── Neon Ball Cyberpunk Corridor (*).png
```

---

## 🕹️ Controls

### Desktop
- **W / Up Arrow:** Accelerate Forward
- **S / Down Arrow:** Brake / Reverse
- **A / Left Arrow:** Steer Left
- **D / Right Arrow:** Steer Right
- **Spacebar:** Jump
- **P / Escape:** Pause / Resume

### Mobile & Touch
- **On-Screen D-Pad:** 4-way movement controls
- **JUMP Button:** Jump over laser mines and platform gaps

---

## 🚀 Deployment & Submission

1. Log in to the [CrazyGames Developer Portal](https://developer.crazygames.com/).
2. Navigate to your game dashboard: **Neon Core** (`AWAITING REVIEW`).
3. Click **"Submit new version"**.
4. Upload `build/neon_core_crazygames_v2.zip` (or `index.html`).
5. Update media with the included 16:9, 2:3, and 1:1 covers from `media/covers/` and videos from `media/videos/`.
6. Submit for review!
