# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static personal landing page for Alem Šabić, built with vanilla HTML, CSS, and no external dependencies or build process. The site features a split-screen layout with a profile image on the left and content on the right.

## Architecture

- **Single-file application**: All HTML, CSS, and structure is contained in `index.html:1-140`
- **No build process**: The site is served directly as static HTML
- **Assets**: Profile image (`alemsabic.png`) is referenced directly in the CSS background

## Development

### Running locally
```bash
# Option 1: Using Python's built-in server
python3 -m http.server 8000

# Option 2: Using any static file server
# Then open http://localhost:8000 in browser
```

### Making changes
Simply edit `index.html` and refresh the browser. No compilation or build step required.

## Code Structure

- **Styling**: Embedded in `<style>` tag (index.html:7-117)
  - Dark theme with color scheme: background `#141516`, text `#f6f6f6`, accent `#47bec7`, hover `#F44336`
  - Responsive breakpoint at 968px switches from side-by-side to stacked layout
  - System font stack for native appearance

- **Layout**: Split-screen design (index.html:120-138)
  - `.image-side`: Left half with background image
  - `.content-side`: Right half with centered content
  - Flexbox-based responsive layout

- **Content sections**:
  - Main heading with name
  - Intro paragraph (currently placeholder text)
  - "Kontakt" section with email and LinkedIn links

## Important Notes

- The intro text (index.html:127) contains placeholder "Lorem ipsum" text that should be replaced with actual content
- Email link (index.html:132) is currently a placeholder `#` that needs a real mailto link
- Site is in German language (`lang="de"` in index.html:2)
