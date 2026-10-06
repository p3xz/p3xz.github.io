# Phoenixfy | Namish Yadav

Phoenixfy is the personal hub and link-in-bio site of Namish Yadav (p3xz): contact links, socials, and app-mod install guides, all on one page. Live at https://p3xz.github.io

## Why

One page to point everyone to: all his contact links and social profiles in a single place, plus the Instagram mod install guides he shares often, so they do not have to be re-explained one chat at a time.

## When

Built in December 2024.

## What we used

![HTML](https://skillicons.dev/icons?i=html) ![CSS](https://skillicons.dev/icons?i=css) ![JavaScript](https://skillicons.dev/icons?i=js)

- HTML5, CSS3, JavaScript (vanilla ES6+, no frameworks or build tools)
- Styling: custom CSS (833 lines, CSS custom properties for theming) with Google Fonts (Poppins, Montserrat, Qwitcher Grypen, Great Vibes, Parisienne)
- Hosting: GitHub Pages, served as a fully static site with no backend and no dependencies to install
- Extras: robots.txt and sitemap.xml for search indexing, Open Graph and Twitter meta tags, SVG favicon

## Why we used this

- Plain HTML/CSS/JS with no build step, so the site deploys straight to GitHub Pages by pushing to the main branch.
- Vanilla JavaScript is enough for everything interactive here: theme toggle, toast, copy-to-clipboard, expandable guides. No framework overhead.
- CSS custom properties power the dark/light theme swap from one variable set, flipped at runtime by script.js.

## How it works

- One index.html, one style.css, one script.js. Everything runs in the browser, with no server side logic and no build.
- The loading screen animates with a live progress counter, then the parallax PHOENIXFY hero renders with layered edge and glow text that follows the cursor. A star trail effect follows the mouse on desktop.
- The theme toggle flips CSS variables via classList, swapping the animated background and accent colors between light and dark.
- The Discord button copies the username to the clipboard and shows a toast notification.
- The MODS guides are expandable sections: Android covers AeroInsta V24.0.0 with step-by-step screenshots; iOS covers InstaKilloGram with a Scarlett sideloading walkthrough, screenshots, and video tutorial links.

## Features

Home: animated loading screen with a live progress counter and a rotating image stack, then a parallax PHOENIXFY hero with layered edge and glow text that follows the cursor. A star trail effect follows the mouse on desktop.

Navigation: fixed nav bar with smooth-scroll links to Home, Contact, MODS, and Privacy, a dark/light theme toggle that swaps the animated background and accent colors, and a hamburger menu with a slide-in panel on mobile.

Contact: profile card with bio and link buttons for Instagram (main and private), Telegram, Discord, and email. The Discord button copies the username to the clipboard and shows a toast notification.

MODS: expandable guides for installing Instagram mods. Android covers AeroInsta V24.0.0 with step-by-step screenshots; iOS covers InstaKilloGram with a Scarlett sideloading walkthrough, screenshots, and video tutorial links.

Privacy: dedicated section documenting that the page is fully static, stores nothing, sets no cookies, and runs no analytics or tracking.

Footer: credit line plus social links to GitHub, LinkedIn, Instagram, portfolio, and privacy.

SEO: meta description, canonical URL, Open Graph and Twitter card tags, robots.txt, and sitemap.xml.

## Getting Started

No build step and no dependencies. Clone the repo and open index.html in any browser, or serve the folder with a static server:

```
git clone https://github.com/p3xz/p3xz.github.io.git
cd p3xz.github.io
python3 -m http.server 8000
```

Then visit http://localhost:8000

Deploying to GitHub Pages: push to the main branch and the site goes live at https://p3xz.github.io automatically.

## Credits

Built by Namish Yadav (https://github.com/p3xz). Released under the MIT License (see LICENSE).
