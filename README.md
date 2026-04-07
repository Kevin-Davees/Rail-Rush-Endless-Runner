# 🚆 Rail Rush — Endless Runner

Rail Rush is a browser-based **3D endless runner game** built using **Three.js**.  
The player runs along railway tracks, dodging trains and barriers while collecting coins to increase score and multiplier.

This project is part of a **vibe-coding experiment**, and this repository represents **my 4th attempt** at building the game.

The game runs entirely in the browser with **no build tools or frameworks required**.

---

# 🎮 Gameplay

The player runs forward automatically while the environment moves toward them. The goal is to **survive as long as possible**, avoid obstacles, and collect coins.

### Mechanics

- Infinite procedural track generation
- Increasing speed over time
- Three lane movement system
- Jump and slide mechanics
- Coin collection with multiplier system
- Dynamic obstacle spawning
- Particle effects
- 3D environment with buildings and railway tracks

### Obstacles

| Obstacle | Behavior |
|--------|--------|
| Train | Blocks an entire lane |
| Low Barrier | Must **jump** |
| High Barrier | Must **slide** |

### Scoring

Score is based on:

- Distance travelled
- Coins collected
- Coin multiplier progression

Multiplier increases as more coins are collected.

---

# 🎮 Controls

### Keyboard

| Action | Keys |
|------|------|
| Move Left | `←` or `A` |
| Move Right | `→` or `D` |
| Jump | `↑`, `W`, or `Space` |
| Slide | `↓` or `S` |
| Start / Restart | `Space` or `Enter` |

### Mobile

| Action | Gesture |
|------|------|
| Move Left | Swipe Left |
| Move Right | Swipe Right |
| Jump | Swipe Up |
| Slide | Swipe Down |

---

# 🧠 Technical Overview

The entire game currently runs from a **single HTML file** and uses **Three.js** for rendering.

### Core Systems

- **Game Loop**
  - Uses `requestAnimationFrame`
  - Handles physics, collisions, spawning and rendering

- **Procedural World**
  - Track chunks spawn ahead of the player
  - Old chunks are recycled

- **Physics**
  - Gravity system for jumping
  - Slide timer
  - Lane switching interpolation

- **Collision Detection**
  - Uses `THREE.Box3` bounding boxes

- **Dynamic Difficulty**
  - Speed increases over time
  - Obstacle spacing decreases

- **Particle System**
  - Coin collection effects
  - Crash effects on game over

---

# 🧱 Built With

### Core Technologies

- HTML5  
- CSS3  
- JavaScript  

### Rendering Engine

- Three.js (r128)

### Graphics

- WebGL via Three.js  
- Procedural geometry  
- MeshStandardMaterial lighting  

### Game Architecture

- Vanilla JavaScript
- No external game engines
- No build pipeline

---

# 📁 Project Structure (Current)

```
rail-rush/
│
├── Final.html        # Main game file
├── README.md         # Project documentation
│
└── (future files)
```

More files and improvements will be added later.

---

# 🚀 Running the Game

### Option 1 — Open Locally

Simply open the HTML file in your browser:

```
Final.html
```

### Option 2 — GitHub Pages

If hosted with GitHub Pages:

```
https://yourusername.github.io/repository-name/
```

---

# 📈 Future Improvements

Planned improvements include:

- Sound effects and background music
- Better player animations
- Power-ups
- Score persistence
- Mobile UI improvements
- New obstacle types
- Environment variety
- Optimization for low-end devices

---

# ⚠️ Notes

- The game currently prioritizes **gameplay feel and experimentation** rather than full production polish.
- This repository represents **iteration #4** of the project.
- The project will continue evolving with new systems and files added over time.
