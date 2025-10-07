# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static landing page for **autosapien.ai**, a "coming soon" site hosted on GitHub Pages. The site features:
- A cyberpunk-themed landing page with the tagline "AI THAT LEARNS AND EVOLVES"
- An embedded MS-DOS Pac-Man game from archive.org
- Custom domain: www.autosapien.ai (configured via CNAME)

## Architecture

**Single-file static site**: The entire site is contained in `index.html` with inline CSS and JavaScript. No build process, dependencies, or package manager is used.

**Key components**:
- HTML structure with embedded game iframe
- CSS styling with cyberpunk theme (dark background #0d0d0d, cyan accent #00a0aa)
- Loading spinner animation that hides when game iframe loads
- CNAME file for GitHub Pages custom domain configuration

## Development

**Local development**: Open `index.html` directly in a browser. No server required for basic viewing, though some features (like iframe loading) may require a local HTTP server.

**Quick local server**:
```bash
python -m http.server 8000
# or
python3 -m http.server 8000
```

**Testing changes**: Simply edit `index.html` and refresh the browser.

## Deployment

This site is deployed via GitHub Pages. Changes pushed to the `main` branch are automatically published.

**Deploy workflow**:
1. Edit `index.html`
2. Commit changes: `git add index.html && git commit -m "description"`
3. Push to main: `git push origin main`
4. GitHub Pages will automatically update the site at www.autosapien.ai

## File Structure

- `index.html` - Main landing page (all HTML, CSS, JS inline)
- `CNAME` - Custom domain configuration for GitHub Pages
- `README.md` - Basic repository information
- `ROBOT LOGO.PNG` - Logo asset (not currently used in site)
- `.obsidian/` - Obsidian vault configuration (unrelated to website)

## Style Guide

When editing the site, maintain:
- Cyberpunk/terminal aesthetic
- Color scheme: dark background (#0d0d0d), cyan primary (#00a0aa), gray secondary (#666666, #999999)
- Monospace font (Courier New)
- Robot emoji (🤖) as branding element
