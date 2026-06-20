# 🏎️ Turbo Dash

A fast, kid-friendly arcade racer that runs in any browser — **no install, no build step, no assets**. The whole game is a single `index.html` file (HTML + Canvas + Web Audio).

Dodge obstacles, grab coins, chain near-misses to fill your boost, and unlock new racers and worlds.

## ▶️ Play it

**Just double-click `index.html`** — it opens in your default browser and plays immediately.

Or serve it locally:

```bash
npx http-server -p 8123 -c-1
# then open http://localhost:8123/index.html
```

## 🎮 Controls

| | 3D view | Side view |
|---|---|---|
| Steer / move | `←` `→` | `↑` `↓` |
| Speed up | `↑` | `→` |
| Slow down (to dodge & grab coins) | `Space` / `↓` | `Space` / `←` |
| Pause | `P` | `P` |
| Mute | `M` | `M` |
| Restart after a crash | `Space` / `Enter` | `Space` / `Enter` |
| Back to menu (after crash) | `Esc` | `Esc` |

## ✨ Features

- **Two views:** a pseudo-**3D perspective road** with drawn, shaded vehicles, scenery, and obstacles — or a classic **side-scroller**. Pick on the menu (your choice is remembered).
- **6 racers:** Race Car, Tiger, Lion, Monster Truck, Dino, Creeper (animals/characters ride a kart in 3D).
- **5 worlds:** City, Jungle, Lava, Mountains, Minecraft — each with its own sky, road, scenery, and obstacles.
- **Escalating speed** the further you go, so it keeps getting more intense.
- **Near-miss → Boost loop:** skim past obstacles to fill the boost meter; when full it auto-fires a speed surge with double points.
- **Coins & unlocks:** coins you collect bank between runs and unlock new racers and worlds.
- **Per-run goals** for bonus coins, combos, milestones, particle effects, sound effects, and a saved high score.

## 🛠️ Tech

- Single self-contained `index.html` — no dependencies, no bundler.
- Rendering: HTML5 Canvas 2D. Audio: Web Audio API (procedurally generated, no sound files).
- Progress (best score, coins, unlocks, settings) is stored in `localStorage`.

## 📄 License

[MIT](LICENSE) — free to use, modify, and share.
