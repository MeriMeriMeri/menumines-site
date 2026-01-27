# MenuMines Marketing Site

Marketing website for [MenuMines](https://menumines.com), a macOS menu bar app for daily Minesweeper puzzles.

## Overview

MenuMines gives you one Minesweeper puzzle every day, right in your menu bar. The same board is generated for everyone on Earth, so you can compare times with friends.

This repo contains the static marketing site, currently deployed on **GitHub Pages**.

## Tech Stack

- Plain HTML (single `index.html`)
- [JetBrains Mono](https://www.jetbrains.com/lp/mono/) font via Google Fonts
- All CSS is inline (no external stylesheet dependencies)
- No build step required

## Local Development

Open `index.html` in a browser:

```sh
open index.html
```

Or use any local server:

```sh
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deployment

The site is deployed via [GitHub Pages](https://pages.github.com/) from the `main` branch. Pushing to `main` triggers a deploy automatically.

## Project Structure

```
.
├── index.html    # The entire marketing site
└── README.md
```
