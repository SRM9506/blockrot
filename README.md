# BLOCKROT

Open-world 3D zombie survival roguelite, playable in the browser. Boxhead-inspired, Vampire Survivors-influenced. Built with Three.js (r128), vanilla JavaScript, procedural audio, and zero external assets — the entire game ships as a single HTML file.

**Play:** open `blockrot.html` in any modern browser. Desktop (mouse/keyboard), gamepad, and mobile touch are all supported.

## Features

- **Massive open maps** — 3 zones (urban sprawl, cursed graveyard, frozen valley), each with procedural prop layouts, sky domes, horizon silhouettes, and weather
- **16 weapons** — 7 base weapons with 7 stat-triggered evolutions, plus 9 exclusive weapons pulled from a relocating **Mystery Box** (escalating cost, CoD-zombies style)
- **8 enemy types** — walkers, runners, brutes, spitters, exploders, armored tanks with rear weak spots, necromancers, and a 3-phase boss with telegraphed charge attacks
- **Roguelite progression** — XP gems, 16 in-run upgrades with Common/Rare/Epic rarities, boss reward chests, coins banked into a permanent meta shop (7 upgrades incl. GRIT second-chance)
- **6 operatives with ultimates** — 2 unlockable, each with a kill-charged ultimate ability
- **8 achievements → cosmetics** — tracer colors and character skins
- **Daily seeded runs** with separate local leaderboard
- **Full input support** — mouse/keyboard, gamepad (twin-stick), and mobile touch (virtual joystick, drag-aim, aim-assist toggle)
- **Procedural everything** — dark synthwave soundtrack and all SFX generated via Web Audio, all models built from primitives, no asset files

## Controls

| Action | Keyboard/Mouse | Gamepad | Touch |
|---|---|---|---|
| Move | WASD | Left stick | Left joystick |
| Aim | Mouse | Right stick | Drag right side |
| Fire | Left click | RT | FIRE button |
| Jump | Space | A | JUMP button |
| Dash | Ctrl / V | B | DASH button |
| Ultimate | F | Y | ULT button |
| Weapons | 1–0 / Q / E / scroll | Bumpers | Tap slots |
| Pause | P / Esc | Start | Tap minimap |

## Status

Active development. This is the single-file prototype ("design lab") phase; the roadmap is a Vite + ES modules restructure, an itch.io playtest build, and eventually Steam via an Electron wrapper. See `logs/` for session-by-session development history.

## Tech notes

- Three.js r128 (CDN) — no CapsuleGeometry/OrbitControls in this release, so all geometry is primitive-composed
- Persistence via a safe localStorage wrapper (falls back to in-memory when sandboxed)
- No build step, no dependencies, no assets — view source is the whole game
