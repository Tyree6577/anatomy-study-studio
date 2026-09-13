# Anatomy Study Studio
A static, browser-local Anatomy & Physiology I study application.

Serve `dist/` over HTTP (for example, `python3 -m http.server 4173 --directory dist`). No package installation, server database, account, API key, or AI grading is required.

- `dist/data.js`: curated questions, explicit alternatives, explanations, references, scope.
- `dist/engine.js`: normalization, scoring, spaced-review schedule, backup validation.
- `dist/diagrams.js`: original SVG teaching schematics.
- `dist/app.js`: accessible study flows, four activities, local persistence.
- `dist/style.css`: responsive visual design.

Browser data uses the localStorage key `anatomy-studio-v1`. Export and import from Progress. Only complete sessions are recorded. No personal results are embedded in the source. Keep a backup before clearing browser storage or changing origins.

## Content limitations
The only supplied attachment was a text brief; the referenced worksheet images were absent. Worksheet-specific handwritten answers and organ-region associations are unverified and excluded. The written list sets the scope. General facts are checked against linked OpenStax references. Original schematics cover major compartments, regions, generic serous layers, urinary organs, and female internal reproductive structures. Other structures use text recall pending reliable identification views. Diagrams are teaching schematics, not realistic lab specimens.

## Validation
175 prompts, every listed term covered. Canonical answers and all aliases validated; wrong near-matches rejected. Review spacing, same-day mastery guard, sorting isolation, invalid-backup rejection and serialization checked. Browser checks completed practice, lab submission, Pinpoint, Region Builder, Term Trail, and System Sort (including pancreas, ovaries, testes). Backup import persisted across reload; export and reset controls checked. Desktop and 390px phone layouts inspected. WebMCP read/start tools validated with valid and invalid input.
