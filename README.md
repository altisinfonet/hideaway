# Hideaway

Hideaway is a website project. This repository holds its source code and project documentation.

> **Status:** early stage. The repository currently contains only this README, so the sections below describe how the project is organized and how to contribute. The setup and usage sections will be filled in as the codebase takes shape.

## Getting started

### Prerequisites

The required tools will be listed here once the tech stack is chosen (for example, Node.js, a package manager, or a static site generator).

### Installation

```bash
git clone https://github.com/altisinfonet/hideaway.git
cd hideaway
```

Install steps for dependencies will be added here.

### Running locally

Instructions for starting a local development server will be added here.

## Project structure

```
hideaway/
├── README.md        Project overview
└── jhargram/        Standalone Jhargram page (publish at /jhargram/)
    ├── index.html   Page markup, styles and scripts (no build step)
    ├── assets/      Ortica Linear and Jost fonts, logo mark and favicon (fonts are self-hosted; no Google Fonts request)
    ├── .htaccess    Optional Apache caching/security headers
    └── images/      WebP photos (rooms/, balconies/, exterior/, grounds/, renders/, plus thumbs/); og-image.jpg is the one JPEG, kept for social-sharing previews
```

The Jhargram page lives outside WordPress and mirrors the main site's design tokens: Ortica Linear (headings, weight 300, -1px tracking) and Jost (body), ink `#153d4b`, background `#f2f2ec`, accent `#e49951`, 12px/600 uppercase pill buttons, 75px side gutters at 1440px. Keep those in sync if the main site's theme changes.

To preview it, serve the repo root over HTTP (for example `python3 -m http.server`) and open `/jhargram/`; opening the file directly works but blocks the web font. To add a photo to its gallery, save a ~1600px WebP (quality ~76) and a ~700px thumbnail (in a `thumbs/` folder next to it) and add `<button data-cat="rooms" data-full="images/rooms/NAME.webp"><img src="images/rooms/thumbs/NAME.webp" alt="..."></button>` inside `#gallery-grid`. `data-cat` is one of `rooms`, `balconies`, `exterior`, `grounds`, `dining`, `drinks` or `renders`.

## Contributing

1. Create a branch from `main` for your change.
2. Make your changes with clear, focused commits.
3. Push your branch and open a pull request describing what changed and why.

## License

No license has been chosen yet. Until one is added, all rights are reserved by the repository owner.
