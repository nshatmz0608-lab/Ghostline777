# GHOSTLINE: Official Showcase Website

A multi-page promotional website for **Ghostline**, a fictional underground street racing game set in the night streets of Los Santos. Built as the DAM50403 Website Design Final Project. The design draws on AAA mobile racing game landing pages: dark, metallic and neon.

## Pages

| File | Purpose |
| --- | --- |
| `index.html` | Home: cinematic hero, story synopsis, game highlights, pre-register CTA |
| `vehicles.html` | Fleet & Customization: 4 car profiles with tier badges and stat bars |
| `gallery.html` | Gameplay & Media: 6-shot gallery with hover zoom, embedded trailer |
| `contact.html` | Download links, Mobile/PC system requirements, developer profile, contact form, social links |
| `thank-you.html` | Confirmation page shown after the contact form is submitted |

All pages share one stylesheet, `style.css`, plus the same header, footer, colors and typography.

## Technologies

- Semantic HTML5 and vanilla CSS3. No JavaScript at all: the mobile menu is a pure-CSS checkbox toggle.
- Google Fonts: **Orbitron** (display) and **Rajdhani** (body).
- CSS Grid layouts, `clamp()` fluid type, `@media` breakpoints at 1100px, 960px and 640px.
- CSS animations: staggered hero entrance, ticker marquee, animated stat bars, scroll-driven reveals (in supporting browsers), plus `prefers-reduced-motion` support.
- **Netlify Forms** handles the contact form. Submissions show up in the Netlify dashboard under *Forms → contact*.

## Design principles

- **Balance**: symmetrical grids (car cards, spec tables) are paired with asymmetrical ones (offset highlight cards, zig-zag customization list, mosaic gallery). All of them collapse to a single column on mobile.
- **Contrast**: `#0b0b0b` / `#121212` backgrounds with `#ffffff` text. Accent colors are `#ff003c` (red) and `#00f0ff` (cyan).
- **Unity**: the same glass navbar, chrome logo, angled-corner shapes, fonts and footer appear on every page.

## Running locally

Open `index.html` in a browser. All image paths are relative (`images/filename.jpg`). The contact form only stores submissions once the site is deployed on Netlify.

To preview with Netlify features locally, run `netlify dev`.

## Customizing

- **Trailer**: the YouTube embed on `gallery.html` points to a stand-in racing trailer. Replace the video ID in the `iframe` `src` with the real Ghostline trailer.
- **Images**: replace any file in `images/` with one of the same name.
- **Credits**: edit the footer `credits` block to add student name(s) and ID(s).
