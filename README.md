# Maze0

Two browser-based 3D maze RPGs — no installation, no server required. Open either HTML file directly in Chrome or Edge.

> **Maze_Action_3D** was most recently updated with a new Arena survival map, a flying Dragon boss, and fully procedural 3D walking sprites for all ground monsters.

---

## Games

### Maze_Action_3D — Real-time Action
Move, look around, and attack in real time. Monsters chase and strike automatically when adjacent.

### Maze_Turn_3D — Turn-based Combat
Every move is a turn. When you step next to a monster the game enters turn-based combat — attack, use your ability, then wait for the enemy to retaliate.

---

## Features

- **Three.js WebGL rendering** — perspective 3D walls with procedural textures, ambient + point lighting
- **2D sprite overlay** — monsters, items, and the 🌀 portal projected onto a transparent canvas layer on top of the 3D scene
- **Procedural 3D walking sprites** — ground monsters are fully canvas-drawn (8-frame animation) with spherical bodies, cylindrical limbs, specular shading, and human-like arm swing (foreshortening for depth)
- **Procedural Web Audio BGM** — 3-chord progressions synthesised entirely in the browser (no audio files); explore and combat variants switch automatically; title screen music plays on first click
- **4 maze themes** — Space 🚀, Forest 🌿, Candy 🍬, and Arena 🏟️ — each with unique wall textures, floor colours, and BGM
- **Arena survival map** — endless waves of monsters in a Roman colosseum under a procedural night sky; no exit portal, fight until you fall
- **4 playable characters**

| Character | Weapon | Special Ability |
|-----------|--------|-----------------|
| 🐰 Rabbit  | Twin Daggers 🗡️ | Backstab — burst damage from stealth |
| 🐔 Chicken | Broad Sword ⚔️  | Battle Cry — AoE damage boost |
| 🐭 Mouse   | Arcane Staff 🪄 | Fireball — ranged projectile |
| 🐯 Tiger   | Holy Sword ✨   | Divine Shield — temporary invincibility |

- **4 monster types**

| Monster | Ability | Notes |
|---------|---------|-------|
| 👾 Red Spook | Shadow Bolt 💀 | Procedural 3D sprite — red sphere body, cycloptic eye, clawed arms |
| 👹 Boca      | Poison Cloud ☠️ | Procedural 3D sprite — fluffy green, two huge eyes, paw arms |
| 👺 Imp       | Inferno Strike 🔥 | Procedural 3D sprite — metallic blob, red bat wings |
| 🐉 Dragon    | Fire Breath 🔥 | Flies in orbit above the arena; canvas-drawn wing-flap animation; appears from wave 3 |

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

> **Maze_Turn_3D** uses the same controls but space/click is replaced by menu-driven turn choices during combat.

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
