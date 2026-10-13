# VETT VINU

A mobile-first mini-game arcade built with React, TypeScript, Vite, and CSS. Player profiles and match history are stored in the current browser's `localStorage`; there is no backend or database.

## Run locally

Requires Node.js 20 or newer.

```bash
npm install
npm run dev
```

## Verify and build

```bash
npm run typecheck
npm run build
npm run preview
```

The production build is written to `dist/`.

## Deploy to Vercel

1. Push this project to a GitHub repository.
2. Import that repository in Vercel.
3. Keep the detected Vite framework setting, with `npm run build` as the build command and `dist` as the output directory.

The included `vercel.json` records these settings.

## Games

- SOS (local two-player)
- Tic-Tac-Toe (computer or local player)
- Dots & Boxes (local two-player)
- Minesweeper
- Memory Match
- Reaction Test
- Snake
- Maze Runner

## Storage and leaderboard limitations

A first-time player enters a name, which is remembered in the same browser on the same device and site origin. Game history, achievements, personal records, and settings start empty and update from actual play. Opening a preview URL versus the deployed Vercel URL counts as a different origin, so the profile does not automatically transfer. Clearing browser site data can remove this local profile. A Vercel-hosted static app cannot sync scores between players or devices without a backend/database; the leaderboard in this version is therefore a local personal-record list, not a global leaderboard.

## Accessibility and privacy notes

The app does not ask for an email, account, or password and does not send game history to a server. Game boards include tap/click controls, and keyboard controls are provided for selected games.
