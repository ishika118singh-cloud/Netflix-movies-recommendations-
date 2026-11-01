# Netflix Movies Recommendations

A single-page movie recommendation web app that helps users discover movies based on mood and preferred genres.

## Overview

This project provides a polished UI flow where users:
1. Select their current mood
2. Pick one or more genres
3. Receive curated movie recommendations

The app attempts to fetch recommendations from Anthropic and gracefully falls back to a built-in movie list if an API response is unavailable.

## Features

- Mood-based recommendation flow
- Multi-select genre filtering
- Interactive movie cards with save-to-favorites support
- Client-side filters (search, rating, and release decade)
- “Surprise Me” option for random picks
- Direct links to Netflix or JustWatch search
- Fully static frontend (HTML, CSS, JavaScript)

## Project Structure

- `/index.html` – Main and complete application file
- `/Netflix app index.html` – Alternate copy of the app file

## How to Run

Because this is a static project, no build step is required.

### Option 1: Open directly
- Open `index.html` in your browser.

### Option 2: Use a local static server (recommended)
From the project root, run one of the following:

```bash
python -m http.server 8000
```

Then open:

- `http://localhost:8000/index.html`

## Customization

You can tailor recommendations by editing:
- Mood options in the Step 1 section
- Genre options in the Step 2 section
- Fallback movie data in `getFallbackMovies()`

## Notes

- If no external API credentials/configuration are provided, fallback recommendations are shown.
- No external build tools or package managers are required.
