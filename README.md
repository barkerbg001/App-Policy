# App-Policy

This repository contains standalone HTML privacy policy pages for several apps, plus a small index that serves as a centralized hub.

What's included
- `index.html` — Privacy Policy Hub: a small control hub with cards linking to each app's policy.
- `styles.css` — Centralized stylesheet used by all pages (dark-mode aware, CSS variables, shared components).
- Individual policy pages:
	- `retain.html` (Retain — note-taking app)
	- `barkify.html` (Barkify)
	- `calculator.html` (CalculatorApp)
	- `dadjokesgalores.html` (Dad Jokes Galore)
	- `insultmaster.html` (Insult Master)
	- `nextmcu.html` (Cineverse)

Quick start
1. Open `index.html` in your browser to view the Privacy Policy Hub. From there click any card to open a specific policy page.
2. To preview locally with live-reload, use the VS Code Live Server extension or serve the folder with a simple HTTP server:

```bash
# from the repo root
python3 -m http.server 8000
# then open http://localhost:8000/index.html
```

Notes for maintainers
- The visual style is centralized in `styles.css`. Pages can request a brand accent color by adding `data-accent="<name>"` to the `<body>` element (examples: `data-accent="barkify"`, `data-accent="cineverse"`).
- When adding new policy files, update `index.html` to include a card link for each new file (or ask me to implement an automated generator).

Contributing
- Send PRs for content changes or new policy pages. Keep page filenames relative and ensure pages link `styles.css`.

License
- See `LICENSE` in the repo root.
