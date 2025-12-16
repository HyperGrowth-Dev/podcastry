# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Podcastry is a static landing page for an on-demand podcast studio service. The entire site is a single `index.html` file deployed on Vercel.

## Tech Stack

- Single HTML file with inline CSS and JavaScript
- Tailwind CSS via CDN (`cdn.tailwindcss.com`)
- Lucide icons via CDN (`unpkg.com/lucide`)
- Google Fonts: Oswald (headings) and Inter (body)

## Development

No build process. Open `index.html` directly in a browser or use any local server:
```bash
npx serve .
# or
python -m http.server 8000
```

## Architecture

- **Styling**: Custom CSS variables for brand colors (`--brand-mint: #4FFFB0`, `--brand-black: #111111`) with Tailwind utility classes
- **Forms**: Two waitlist signup forms (hero and CTA sections) that POST to a Zapier webhook
- **Icons**: Initialized via `lucide.createIcons()` on page load

## Brand Guidelines

- Primary mint color: `#4FFFB0`
- Background black: `#111111`
- Headings use Oswald font, uppercase
- Bold "neo-brutalist" style with offset shadows (e.g., `shadow-[8px_8px_0px_#4FFFB0]`)
