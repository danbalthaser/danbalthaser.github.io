# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a personal portfolio website for Daniel Balthaser, hosted on GitHub Pages. The site serves as a landing page linking to various projects, resume, photography portfolio, and social media profiles.

**Repository**: https://github.com/danbalthaser/danbalthaser.github.io
**Hosted at**: danbalthaser.com (via CNAME)

## Architecture

### Static Site Structure

This is a simple static HTML site with no build process or server-side rendering:

- **Root files**: `index.htm` (landing page), `resume.htm` (resume page), `favicon.ico`
- **CSS**: `css/` directory contains stylesheet files
  - `index-stylesheet.css` - Landing page styles
  - `resume-stylesheet.css` - Resume page styles
- **Applications**: `appserve/` directory contains multiple self-contained applications/demos (Snake, PandoraSmall, port_scanner, telnet, mbr, HyperText)
- **Static assets**: `images/` and `documents/` directories

### Page Layout (index.htm)

The landing page uses a two-column layout with intentional formatting (left and right sections without whitespace between them to prevent wrapping). Key elements:
- Left section: Empty div (used as visual space)
- Right section: Name area with social media and external links
- Uses Font Awesome icons for social links and FontRoboto for typography

## Development

### Common Tasks

Since this is a static site with no build process:

- **View locally**: Open `index.htm` or `resume.htm` directly in a browser, or serve via a simple HTTP server: `python3 -m http.server 8000`
- **Edit content**: Directly modify HTML files in the root directory
- **Update styles**: Edit files in the `css/` directory
- **Add images/documents**: Place files in `images/` or `documents/` directories and link from HTML

### Git Workflow

- **Main branch**: `master`
- **Remote**: `origin` (danbalthaser/danbalthaser.github.io)
- Changes pushed to `master` are automatically deployed to GitHub Pages

## Key Notes

- **No build tools**: This is plain HTML/CSS with no compilers, bundlers, or preprocessors
- **Format preservation**: The HTML in `index.htm` has deliberate formatting (no whitespace between left and right divs) to prevent layout issues
- **Hosted via GitHub Pages**: Site automatically deploys from the `master` branch
- **Domain**: CNAME file points to `danbalthaser.com`
