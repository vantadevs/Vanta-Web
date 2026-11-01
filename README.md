# Vanta Hub website

A responsive, static multi-page website implemented as a small client-side app. No build step or package installation is required.

## Run locally
Open `index.html` in a modern browser, or serve the folder with any static web server (recommended for local testing):
```bash
python -m http.server 8000
```
Then visit `http://localhost:8000`.

## Content management
Edit `app.js`:
- `GAMES`: all 17 supported entries, labels, descriptions and artwork colour tokens.
- `GAME_DETAILS`: add confirmed `freeFeatures`, `premiumFeatures`, and optional `freeLink` per game ID.
- `RECENTLY_ADDED` and `RECENTLY_UPDATED`: add official update objects with `id`, `name`, `date`, `summary` and optional `description`.

The update arrays are intentionally empty and feature arrays intentionally show pending copy until official details are provided. This avoids fabricating release dates, changelogs, or script functionality.

## Functional scope
- Five hash-routed pages: Home, Scripts, Premium, Updates, Contact.
- Working search and combined availability/recent filters.
- Clickable cards and accessible details modal with separate free/premium feature sections.
- Discord invite, ticket links, and `mailto:` support.
- Responsive layouts and keyboard-accessible card/modal interactions.
- No login button because no authentication provider is configured.
- No purchase gateway or email form because no payment/email backend is configured.

## Assets
`assets/vanta-logo.jpg` is the supplied purple Vanta logo. Game cards use original CSS artwork treatments rather than unrelated or unlicensed game images. Replace these with official game thumbnails when you have approved assets.
