# Heenim Catch 💙

A one-thumb arcade game for Super Junior's Kim Heechul — catch the sapphire pearls
the ELF ocean throws up on stage, and dodge the 5AM schedules.

Built as a single self-contained `index.html`: no build step, no dependencies,
no server needed. Open the file and play.

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

Deployment is automatic: `.github/workflows/pages.yml` publishes the repository
root to GitHub Pages on every push to the default branch.

## Files

- `index.html` — the whole game: styles, canvas renderer, game loop, WebAudio SFX
- `manifest.json` — PWA metadata for home-screen install
- `icon.svg` — app icon
- `preview.png` — link preview shown when the URL is pasted into a chat
- `.github/workflows/pages.yml` — publishes the site to GitHub Pages

A fan project, made for fun. Not affiliated with Super Junior, Label SJ or SM Entertainment.
