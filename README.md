# Portfolio

Personal portfolio website of Cedric Kawczynski, computer science student and software developer.

A single page with a short intro, links to GitHub and LinkedIn, and a list of my personal projects.

## Tech Stack

- [Astro](https://astro.build)
- Plain CSS
- Hosted on GitHub Pages

## Getting Started

```bash
npm install
npm run dev
npm run build
```

## Adding a Project

Projects are defined in `src/data/projects.json`. Each entry has:

| Field         | Description                     |
| ------------- | ------------------------------- |
| `title`       | Project name                    |
| `subtitle`    | One-line problem statement      |
| `description` | Short description (2–3 sentences) |
| `image`       | Preview image in `public/images/` |
| `tags`        | List of technologies            |
| `url`         | Link to repository or live demo |
| `openSource`  | `true` / `false`, shown as a label on the card |

### Collections

A card can group several similar projects (e.g. game jams). Add an `entries` list instead of a single `url`:

| Field   | Description                       |
| ------- | --------------------------------- |
| `title` | Name of the individual project    |
| `event` | Context, e.g. jam name and year   |
| `team`  | Team size, e.g. `2er-Team`        |
| `url`   | Link to the game / repo (optional) |

Tag colors live in `src/data/tag-colors.json`; tags without an entry are grey.
