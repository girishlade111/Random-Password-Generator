# Random Password Generator

A lightweight, privacy-first random password generator that runs entirely in your browser. Pick your character sets, tune the length, generate strong passwords instantly, and copy them with one click. Nothing is sent anywhere — everything happens client-side.

## Features

- **Customizable length** — slider from short PINs to long passphrases (up to 64+ chars)
- **Character set toggles** — uppercase, lowercase, digits, and symbols; mix and match
- **Strength meter** — live entropy estimate and visual strength indicator
- **One-click copy** — copy the generated password straight to your clipboard
- **Regenerate** — spin up a new password instantly without reloading
- **100% client-side** — uses the browser's `crypto.getRandomValues()` for secure randomness; no network calls, no tracking, no server

## Tech stack

- Plain HTML, CSS, and vanilla JavaScript (single `index.html`, zero dependencies)

## Quick start

Just open `index.html` in any modern browser, or serve the folder locally:

```bash
npx serve .
# then visit the printed URL
```

No build step, no dependencies, no environment variables.

## Project structure

```
.
├── index.html   # Entire app: markup, styles, and password-generation logic
├── LICENSE
└── README.md
```

## How it works

Password characters are drawn from the browser's cryptographically secure random number generator (`window.crypto.getRandomValues()`), so generated passwords are suitable for real use. The strength meter scores passwords by character-set size × length (estimated entropy bits).

## Deploy

Static site — host it anywhere static files work (GitHub Pages, Cloudflare Pages, Netlify drop, plain Nginx). This repo is published via GitHub Pages.

## License

See [LICENSE](./LICENSE).

## Built by Girish Lade

Crafted by **Girish Lade** — check out more free tools and projects at [https://ladestack.in](https://ladestack.in).
