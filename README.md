# ⚔️ Hex and Bow

A self-contained browser RPG demo built with Three.js. Pick your champion and take on the **Guardian of the First Gate** boss fight — playable on desktop, mobile, and gamepad.

> 🚧 **Early prototype** — rough around the edges, but fully playable.

---

## 🎮 Play It

- **Gameplay video:** [Watch on Google Drive](https://drive.google.com/file/d/1sYsqgrMbtqDQHtUEH1QLQ1tDCyBBD6ML/view?usp=drive_link)
- **CodePen:** [codepen.io/OSINT619/pen/dPNgmaR](https://codepen.io/OSINT619/pen/dPNgmaR)
- **Local:** Download HexAndBow.html and open it in any modern browser — no build step needed, but internet access is required (Three.js and all audio/3D assets are loaded from remote CDN/storage).

---

## 🧙 Characters

| Champion | Class | Playstyle |
|---|---|---|
| **Nightshade** | Mage | Spells: Fireball, Frostbolt, Firefrost combo |
| **Erika** | Archer | Abilities: Arrow Fire, Shadow Volley, Arrow Nuke |

Both characters have three abilities on cooldown, a health bar, and full SFX tied to their kit.

---

## ⚔️ The Boss — Guardian of the First Gate

A multi-phase encounter with four escalating thresholds (100% → 80% → 50% → 30% HP). The boss uses:

- **Fireballs & Meteors** — break line of sight behind arena structures to dodge
- **Spike Rings** — run out of the red ground rings before they erupt
- Increasing aggression as HP drops through each phase

---

## 🕹️ Controls

### Desktop (Keyboard + Mouse)

| Input | Action |
|---|---|
| `WASD` | Move |
| `Shift` | Run |
| `Space` | Jump |
| `1` / `2` / `3` | Abilities (auto-target boss) |
| `LMB` / `RMB` drag | Orbit camera |
| `Scroll` | Zoom |

### Gamepad

| Input | Action |
|---|---|
| Left stick | Move |
| Right stick | Look / camera |
| `A` | Jump |
| `X` / `Y` / `B` | Abilities |

### Mobile / Touch

- **Left side** — virtual joystick for movement
- **Right side** — swipe to control camera
- **Right buttons** — three ability buttons + jump

---

## ✨ Features

- **Single-file** — the entire game lives in `HexAndBow.html`; no dependencies to install
- **Three.js r169** with post-processing: Bloom, AfterImage, vignette, and animated film grain
- **Cinematic HUD** — boss phase bar, player health, ability slots with cooldown sweeps
- **Dynamic audio** — Web Audio API with crossfading music (menu → boss fight → victory), looping footstep sounds, and per-ability SFX
- **Octree physics** — capsule-based character controller with collision
- **Intro cutscene** with skip button
- **Death & Victory** screens with stats

---

## 🛠️ Tech Stack

- [Three.js](https://threejs.org/) `r0.169.0`
- GLTFLoader + DRACOLoader (compressed 3D assets)
- FBXLoader (character animations)
- RGBELoader (HDR environment maps)
- EffectComposer (UnrealBloomPass, AfterimagePass, ShaderPass)
- Octree + Capsule (physics / collision)
- Web Audio API (music system, SFX, movement loops)
- Pure HTML/CSS/JS — no framework, no build tools

---

## 🗂️ Project Structure

```
HexAndBow/
└── HexAndBow.html   # Entire game — HTML, CSS, and JS in one file
```

---

## 🚀 Roadmap / Known Issues

This is an early demo. Areas under active development:

- [ ] More enemies and arena variety
- [ ] Expanded ability kits per class
- [ ] Save / progression system
- [ ] More boss phases and encounter types
- [ ] Polish pass on animations and VFX
- [ ] Action bar needs to be sized.

Contributions, issues, and feedback welcome!

---

## 📄 License

Not yet specified — reach out to [Wastetoken](https://github.com/Wastetoken) for usage questions.
Gameplay video = https://drive.google.com/file/d/1sYsqgrMbtqDQHtUEH1QLQ1tDCyBBD6ML/view?usp=drive_link
<img width="2000" height="2000" alt="Hex and Bow Logo" src="https://github.com/user-attachments/assets/2c3a1574-38d4-4c94-a981-c295cce7dfb2" />
You can also find the Codepen here: https://codepen.io/OSINT619/pen/dPNgmaR
<img width="2880" height="984" alt="image" src="https://github.com/user-attachments/assets/218618a0-08ee-4756-8bfb-0faf710a7400" />
<img width="2880" height="994" alt="image" src="https://github.com/user-attachments/assets/5f6faf92-b089-495c-b107-f013a4d3afa5" />
<img width="2880" height="980" alt="image" src="https://github.com/user-attachments/assets/a8a3a19b-9056-4796-a39a-533b75c0d896" />


