# Clean-Matrix

A static website for **Clean-Matrix**, a community-led conservation group that brings people together to keep shared spaces clean and communities healthy.

Built with plain HTML and CSS: no frameworks, build tools or dependencies.

## Getting started

1. Clone the repository:
   ```bash
   git clone <repo-url>
   cd clean-matrix
   ```
2. Open `home.html` in your browser.

For live reload while editing, you can serve the folder with any static server, for example the VS Code **Live Server** extension, or:

```bash
npx serve .
```

## Project structure

```
clean-matrix/
├── home.html      # Landing page: navigation bar and hero section
├── about.html     # About page: story, mission, what we do, values
├── style.css      # All site styles (colour tokens, nav, hero, responsive rules)
└── images/
    └── environment.jpg
```

## Pages

| Page             | Status    |
| ---------------- | --------- |
| `home.html`      | Done (nav + hero) |
| `about.html`     | Done (story, mission, work, values, CTA) |
| `events.html`    | Planned (linked from nav) |
| `volunteer.html` | Planned (linked from nav and hero buttons) |

## Styling

Colours are defined as CSS custom properties at the top of `style.css`. Reuse them instead of hard-coding values:

| Token      | Value     | Use                  |
| ---------- | --------- | -------------------- |
| `--yellow` | `#f2cb3b` | Highlights, accents  |
| `--ink`    | `#14140d` | Main text            |
| `--green`  | `#1f4d2c` | Brand colour         |
| `--red`    | `#d33a2c` | Call-to-action accent |
| `--paper`  | `#fbf8ef` | Page background      |
| `--line`   | `#d8d3c5` | Borders and dividers |

Headings use the Impact font stack, and labels use `'Space Mono', monospace`. The layout switches to a single column below `860px`.

## Contributing

1. Create a branch for your change.
2. Keep pages consistent: copy the existing `<nav class="navbar">` markup into each new page and link `style.css`.
3. Check the page at both desktop and mobile widths before committing.
