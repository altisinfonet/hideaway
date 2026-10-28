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
    └── images/      Optimised photos used by the page
```

To preview the Jhargram page, open `jhargram/index.html` in a browser. To add a photo to its gallery, put the image in `jhargram/images/` and add another `<button data-full="images/NAME.jpg"><img src="images/NAME.jpg" alt="..."></button>` inside `#gallery-grid`.

## Contributing

1. Create a branch from `main` for your change.
2. Make your changes with clear, focused commits.
3. Push your branch and open a pull request describing what changed and why.

## License

No license has been chosen yet. Until one is added, all rights are reserved by the repository owner.
