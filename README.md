<div align="center">

# 🎴 Anotador de Juegos

**A phone-first scorekeeper for game night: Truco, Chinchón, UNO, Escoba, Generala or any game you like.**

[![Live demo](https://img.shields.io/badge/demo-live-2ea44f?style=flat-square&logo=githubpages&logoColor=white)](https://nico-sanchez.github.io/nico-apps-anotador/)
[![pages-build-deployment](https://github.com/Nico-Sanchez/nico-apps-anotador/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/Nico-Sanchez/nico-apps-anotador/actions/workflows/pages/pages-build-deployment)
![PWA](https://img.shields.io/badge/PWA-offline_ready-5A0FC8?style=flat-square&logo=pwa&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-vanilla-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Dependencies](https://img.shields.io/badge/dependencies-none-blue?style=flat-square)

<img src="docs/screenshot.png" alt="Truco game with three players and their scores" width="300">

</div>

## Features

- **Game presets** with a target score; the app announces the first player who reaches it:

  | Preset   | Target |
  | -------- | -----: |
  | Libre    |      — |
  | Truco    |     30 |
  | Chinchón |    100 |
  | UNO      |    500 |
  | Escoba   |     15 |
  | Generala |      — |

- **Any number of players**, each with quick buttons for `-10`, `-1`, `+1`, `+5` and `+10`.
- **Survives a closed tab** — players, scores and the selected game are kept in `localStorage`.
- **Reset or start over** — zero every score, or clear the table for a new match.
- **Works offline** — a service worker caches the app after the first visit.
- **Light and dark** — follows the system colour scheme.

## Install on your phone

Open the [live demo](https://nico-sanchez.github.io/nico-apps-anotador/) and use your browser's **Add to Home Screen** option. It then opens full screen, like a native app.

## Run locally

Service workers need a real origin, so serve the folder instead of opening the file:

```bash
python3 -m http.server 8000
```

Then browse to <http://localhost:8000>.

## Project structure

```text
index.html     UI, styles and game logic
manifest.json  PWA manifest (name, colours, display mode)
sw.js          Cache-first service worker
```

## More apps

Part of a small collection of web apps — see the [apps landing page](https://nico-sanchez.github.io/apps-landing/).
