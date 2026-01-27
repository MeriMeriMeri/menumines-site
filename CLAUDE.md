# MenuMines Marketing Site

## What This Is

Static marketing site for MenuMines, a macOS menu bar Minesweeper app. Single `index.html` file deployed on GitHub Pages.

## Tech Stack

- Plain HTML, no framework, no external CSS dependencies
- JetBrains Mono font via Google Fonts
- All styles are inline in a `<style>` block (utility classes baked in, no Tailwind CDN)
- No build system, no package.json, no bundler

## Architecture

Everything lives in `index.html`. The page sections in order:

1. Hero - ASCII art logo + tagline
2. App preview - Interactive-looking game grid mockup + download CTAs
3. Features - Three cards (daily puzzle, stats/streaks, accessibility)
4. Screenshots - Four game state mockups (fresh, victory, game over, stats)
5. Controls - Keyboard shortcut reference
6. FAQ - Four Q&A items
7. Final CTA - Download buttons
8. Footer - Links to privacy policy, support, press kit

## Styling Conventions

- Dark background gradient: `#1a1a2e` -> `#16213e` -> `#0f3460`
- Primary buttons: purple gradient `#667eea` -> `#764ba2`
- Glass-morphism cards: `rgba(255,255,255,0.05)` with `backdrop-blur`
- All text uses JetBrains Mono
- All styles (custom components + utility classes) are in the `<style>` block at the top of `index.html`
- Class names follow Tailwind naming conventions but are hand-written CSS (no Tailwind dependency)

## Development

No build step. Open `index.html` directly or use any static file server.

```sh
python3 -m http.server 8000
```

## Deployment

GitHub Pages from the `main` branch. Push to `main` to deploy.
