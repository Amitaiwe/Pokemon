# 🎮 Pokémon Web Adventure

> A full-featured browser Pokémon RPG — no downloads, no installs. Just open and play.

**Live:** [amitaiwe.github.io/Pokemon](https://amitaiwe.github.io/Pokemon)

---

## Overview

Pokémon Web Adventure is a single-file, mobile-first Pokémon game built entirely in vanilla HTML/CSS/JavaScript. It pulls live data from [PokéAPI](https://pokeapi.co), stores progress in Firebase, and supports real-time PvP battles between players.

The game spans Generation 1–3 Pokémon, features a 3×3 biome world map, gym progression across 8 cities, and a full Pokédex — all running in your browser with no backend beyond Firebase.

---

## Features

### 🗺️ World & Exploration
- **9-zone biome map** — Forest, Tower, Ocean, Lava, Cave, Electric, Swamp and more, each with type-specific Pokémon
- **Click-to-encounter** — tap the map to find wild Pokémon
- **Shiny Pokémon** — 1% spawn rate with gold sparkle animation and +15% power bonus
- **Rarity system** — Common, Rare, Very Rare, and Legendary spawns

### ⚔️ Battle System
- **Wild battles** — fight or flee before throwing a ball
- **Gym battles** — 8 gyms with increasing difficulty, leader teams, and type-based AI
- **Real-time PvP** — challenge other online players to live head-to-head battles via Firebase
- **Type effectiveness** — full Gen 1–3 type chart (×2 / ×0.5 / ×0 modifiers)
- **Move choice** — Normal Attack vs. Type Move each turn
- **Post-battle summary** — detailed result screen with HP bars, battle log, and score

### 🎒 Collection & Progression
- **Pokédex** — tracks seen and caught Pokémon, filterable by type, ID, or caught status
- **Evolution chains** — auto-marked as caught across the full chain on capture or evolution
- **Evolution Stones** — 2% drop rate from encounters, stored as inventory, usable from player card
- **PC Storage** — store Pokémon beyond your 6-slot team, transfer to/from team
- **Level-up system** — XP distribution across active team after each battle

### 🌐 Multiplayer & Social
- **Firebase auth** — Google Sign-In with cloud save sync across devices
- **Leaderboard** — top players ranked by team power
- **Online presence** — see which players are currently active
- **Cross-device saves** — progress syncs automatically

### 🔊 Sound & Polish
- **Web Audio API** — original chiptune sound effects for encounters, captures, evolutions, battles, and more
- **Sound toggle** — mute/unmute button always visible
- **Confetti** — celebratory effect on gym victories
- **Responsive design** — optimized for mobile and desktop

---

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | Vanilla HTML5 / CSS3 / JavaScript (ES2022) |
| Pokémon Data | [PokéAPI](https://pokeapi.co) (REST) |
| Auth & Database | Firebase Authentication + Realtime Database |
| Hosting | GitHub Pages |
| Audio | Web Audio API (no external files) |

---

## Project Structure

```
index.html        ← entire game in a single file (~4,100 lines)
README.md
```

Everything — HTML, CSS, JS, game logic, UI, sound engine — lives in `index.html`. No build step, no dependencies, no framework.

---

## Getting Started

### Play instantly
Visit [amitaiwe.github.io/Pokemon](https://amitaiwe.github.io/Pokemon) on any device.

### Run locally
```bash
git clone https://github.com/amitaiwe/Pokemon.git
cd Pokemon
# Open index.html in any browser — no server needed
open index.html
```

### Deploy your own
1. Fork this repository
2. Go to **Settings → Pages → Branch: main → / (root)**
3. Done — your version is live at `https://<your-username>.github.io/Pokemon`

---

## Gameplay Guide

### Starting Out
1. Sign in with Google (or continue as guest)
2. Choose your trainer character
3. Pick your starter Pokémon from Gen 1, 2, or 3

### Catching Pokémon
- Tap the arena to encounter a wild Pokémon
- Fight first to weaken it, then throw a ball
- **2% chance** each encounter to find an Evolution Stone or extra Poké Balls

### Gym Progression
- Defeat all 8 gym leaders to become Champion
- Each gym scales in level and team power
- Winning awards badge, balls, and XP

### PvP Battles
- Tap **קרב אונליין** to find an opponent
- Both players choose a move simultaneously each turn
- Move types: 👊 Normal or ✨ Type (applies effectiveness multiplier)
- 15-second timer per turn — auto-move if time expires

---

## Pokémon Coverage

- **Generation 1–3** base Pokémon pool (~350+ species)
- Evolution chains extend into **Gen 4–9** via PokéAPI
- Legendaries available as Very Rare encounters
- Biome-specific spawns ensure type diversity across zones

---

## Credits

- Pokémon data — [PokéAPI](https://pokeapi.co)
- Sprites — [PokéAPI GitHub sprite repository](https://github.com/PokeAPI/sprites)
- Trainer sprites — [Pokémon Showdown](https://pokemonshowdown.com)
- Pokémon is a trademark of Nintendo / Game Freak / Creatures Inc. — this is a fan project with no commercial intent.

---

## License

MIT License — free to use, modify, and distribute.

> Built with ❤️ as a fan project. Not affiliated with Nintendo or Game Freak.
