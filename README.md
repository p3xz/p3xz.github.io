# Phoenixfy

> Phoenixfy is the personal hub and link-in-bio site of Namish Yadav (p3xz), putting his contact links, socials, and Instagram mod install guides on one page so they never have to be re-explained one chat at a time.

![Status](https://img.shields.io/badge/status-active-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)

Live site: https://p3xz.github.io. Built in December 2024.

## Features

- **Home**: animated loading screen with a live progress counter and a rotating image stack, followed by a parallax PHOENIXFY hero with layered edge and glow text that follows the cursor; a star trail effect follows the mouse on desktop.
- **Navigation**: fixed nav bar with smooth-scroll links to Home, Contact, MODS, and Privacy, a dark/light theme toggle that swaps the animated background and accent colors, and a hamburger menu with a slide-in panel on mobile.
- **Contact**: profile card with bio and link buttons for Instagram (main and private), Telegram, Discord, and email. The Discord button copies the username to the clipboard and shows a toast notification.
- **MODS**: expandable install guides for Instagram mods. Android covers AeroInsta V24.0.0 with step-by-step screenshots; iOS covers InstaKilloGram with a Scarlett sideloading walkthrough, screenshots, and video tutorial links.
- **Privacy**: a dedicated section documenting that the page is fully static, stores nothing, sets no cookies, and runs no analytics or tracking.
- **Footer**: credit line plus social links to GitHub, LinkedIn, Instagram, portfolio, and privacy.
- **SEO**: meta description, canonical URL, Open Graph and Twitter card tags, robots.txt, and sitemap.xml.

## Tech Stack

![HTML](https://skillicons.dev/icons?i=html) ![CSS](https://skillicons.dev/icons?i=css) ![JavaScript](https://skillicons.dev/icons?i=js)

- HTML5, CSS3, JavaScript (vanilla ES6+, no frameworks or build tools)
- Styling: custom CSS (833 lines, CSS custom properties for theming) with Google Fonts (Poppins, Montserrat, Qwitcher Grypen, Great Vibes, Parisienne)
- Hosting: GitHub Pages, served as a fully static site with no backend and no dependencies to install
- Extras: robots.txt and sitemap.xml for search indexing, Open Graph and Twitter meta tags, SVG favicon

Why this stack: no build step means pushing to main deploys straight to GitHub Pages; vanilla JavaScript is enough for everything interactive (theme toggle, toast, copy-to-clipboard, expandable guides) with no framework overhead; CSS custom properties power the dark/light theme swap from one variable set, flipped at runtime by script.js via classList.

## Quick Start

### Prerequisites

- A modern web browser. No build tools or dependencies to install.

### Installation

1. Clone the repo:

```bash
git clone https://github.com/p3xz/p3xz.github.io.git
cd p3xz.github.io
```

2. Open `index.html` in any browser, or serve the folder with a static server:

```bash
python3 -m http.server 8000
```

3. Visit http://localhost:8000.

## Usage

Deploy to GitHub Pages by pushing to the main branch:

```bash
git push origin main
```

The site goes live at https://p3xz.github.io automatically.

## Contributing

This is a personal site, but fixes and improvements are welcome. Fork the repo, make your change, and open a pull request.

## License

Released under the MIT License. See LICENSE for the full text.
