# Heechul fan games 💙

Two one-thumb arcade games for Super Junior's Kim Heechul. Each is a single
self-contained HTML file: no build step, no dependencies, no server needed.
Open the file and play.

| Game | File | Live |
|---|---|---|
| **Heenim Catch** — catch the sapphire pearls, dodge the 5AM schedules | `index.html` | https://testtzm.github.io/Test/ |
| **Heenim Tap Rush** — 45 seconds, tap Heechul, never wake the sleeping one | `tap-rush/index.html` | https://testtzm.github.io/Test/tap-rush/ |

---

# Heenim Catch

Catch the sapphire pearls the ELF ocean throws up on stage, and dodge the 5AM
schedules.

## How to play

| | |
|---|---|
| **Move** | Drag anywhere on the screen (or ← → on a keyboard) |
| **💙 Sapphire pearl** | +10 |
| **📸 Visual shock** | +15 |
| **🎤 MC mic** | +25 |
| **🐱 Heebum** | +50 |
| **⭐ Star** | HEENIM MODE — 7 seconds of ×2 points, a magnet, and immunity |
| **⏰ 📋 🦟 Schedules & antis** | −1 life (you get three) |

Catch things in a row to build a combo: every 5 consecutive catches raises the
score multiplier, up to ×5. Dropping a good item resets the combo but costs no
life. Every 450 points promotes you to the next stage — the drops get faster and
the schedules get more frequent, from *Trainee Days* all the way to *Heenim Legend*.

Your best score is saved in the browser it was played in (`localStorage`), so it
survives a reload but doesn't travel between devices.

## Play it / share it

**Live:** https://testtzm.github.io/Test/ — a public link, no login and no install.
Anyone you send it to can just tap and play.

One-time setup, if that link 404s: repository **Settings → Pages → Build and
deployment → Source: Deploy from a branch**, branch
`claude/suju-heechul-mobile-game-iuxxmr`, folder `/ (root)`, **Save**. The site
is live a minute later and republishes on every push.

## Run it locally

```bash
# just open it
open index.html

# or serve the folder, which also enables "Add to Home Screen"
npx http-server . -p 8080
```

## Put it on a phone home screen

Open the live link on the phone and use **Add to Home Screen** — `manifest.json`
makes it launch fullscreen in portrait with no browser chrome, like an app.

GitHub Pages serves the repository root, so every push updates the live game.

## Heenim Tap Rush

A 45-second reaction game on a 3×3 stage of lightstick rings. Tap Heechul as he
pops up, grab Heebum and Kibok for bonuses, catch the gold rings for duo combos —
and never tap the sleeping member. Keep a nickname, chase your best score, and
share a score card when the timer runs out.

Same deal: one file, `tap-rush/index.html`, open and play.

## Files

- `index.html` — Heenim Catch: styles, canvas renderer, game loop, WebAudio SFX
- `tap-rush/index.html` — Heenim Tap Rush, self-contained
- `manifest.json` — PWA metadata for home-screen install
- `icon.svg` — app icon
- `preview.png` — link preview shown when the URL is pasted into a chat
- `.nojekyll` — tells GitHub Pages to serve the files as-is

A fan project, made for fun. Not affiliated with Super Junior, Label SJ or SM Entertainment.
