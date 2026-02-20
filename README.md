# Maze0

Two browser-based 3D maze RPGs — no installation, no server required. Open either HTML file directly in Chrome or Edge.

---

## Games

### Maze_Action_3D — Real-time Action
Move, look around, and attack in real time. Monsters chase and strike automatically when adjacent.

### Maze_Turn_3D — Turn-based Combat
Every move is a turn. When you step next to a monster the game enters turn-based combat — attack, use your ability, then wait for the enemy to retaliate.

---

## Features

- **Three.js WebGL rendering** — perspective 3D walls with procedural textures, ambient + point lighting, distance fog
- **2D sprite overlay** — emoji/image monsters, items, and the 🌀 portal projected onto a transparent canvas layer
- **Procedural Web Audio BGM** — 3-chord progressions synthesised entirely in the browser (no audio files); explore and combat variants switch automatically; title screen music plays on first click
- **3 maze themes** — Space 🚀, Forest 🌿, Candy 🍬 — each with unique wall textures, floor/ceiling colours, and BGM
- **4 playable characters**

| Character | Weapon | Special Ability |
|-----------|--------|-----------------|
| 🐰 Rabbit  | Twin Daggers 🗡️ | Backstab — burst damage from stealth |
| 🐔 Chicken | Broad Sword ⚔️  | Battle Cry — AoE damage boost |
| 🐭 Mouse   | Arcane Staff 🪄 | Fireball — ranged projectile |
| 🐯 Tiger   | Holy Sword ✨   | Divine Shield — temporary invincibility |

- **3 monster types**

| Monster | Ability |
|---------|---------|
| 👾 Spook   | Shadow Bolt 💀 |
| 👹 Boca    | Poison Cloud ☠️ |
| 👺 Crimson | Inferno Strike 🔥 |

- **Items** — HP potions, MP potions, attack power-ups scattered across each floor
- **Minimap**, floating damage numbers, HP bars, XP / level-up system
- **Multi-floor progression** — reach the 🌀 portal to descend deeper; enemies scale with floor

---

## Controls

| Key / Input | Action |
|-------------|--------|
| `W` / `S` | Move forward / back |
| `A` / `D` | Strafe left / right |
| `Q` / `E` or `◀` `▶` | Rotate camera |
| Mouse (pointer-locked) | Look left / right |
| `Left Click` / `Space` | Attack |
| `F` | Use special ability |
| Stand on 🌀 + `Space` / `Enter` | Advance to next floor |

Click the game view to capture the mouse pointer. Press `Esc` to release it.

---

## Tech Stack

| Layer | Technology |
|-------|------------|
| 3D rendering | [Three.js r160](https://threejs.org/) (CDN) |
| 2D HUD / sprites | HTML Canvas 2D API |
| Audio | Web Audio API — fully synthesised, zero audio files |
| Everything else | Vanilla HTML + CSS + JavaScript, single-file per game |

---

## Running Locally

```
git clone https://github.com/YinchenChang/Maze0.git
cd Maze0
# Open in browser — no build step needed
start Maze_Action_3D.html
start Maze_Turn_3D.html
```

> Chrome and Edge are recommended. Firefox works but pointer-lock behaviour may differ slightly.
