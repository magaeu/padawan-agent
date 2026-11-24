# Project

A profile card to demonstrate build AI agents

# Parts:

- Description of the profile (no max than 20 words).
- Current profession
- Contact information (only email - in a format: example at domain)
- Keywords based on description and profession (in format: #keyword)

# Document structure

- `<!doctype html>`, `<html lang="en">`, `<meta charset="utf-8">`, viewport meta `width=device-width, initial-scale=1`
- `<title>` is the page title
- Landmarks in this order: `<main>` > `<article aria-labelledby="profile-name">` > svg, `<header>` with `<h1 id="profile-name">`, `<p>` description, `<p>` profession, `<address>` contact, `<ul>` keywords

# Image

- Inline SVG, not `<img>`, viewBox `0 0 64 64`, width and height 50
- Content: a developer figure with a `</>` laptop icon, with no `<title>` element
- `role="img"` and a descriptive `aria-label`
- Centered with `display: block; margin: 8px auto`

# Page

- Page background `#f3f4f6`, font Arial, Helvetica, sans-serif
- `body`: margin 0, padding 8px, grid with `place-items: center`
- `main`: width 100%, flex, centered

# Card

- `width: 400px; max-width: calc(100% - 16px); margin: 8px; padding: 8px`
- Border `1px solid #e5e7eb`, top border `4px solid #1D4ED8`, radius 12px
- Shadow `0 8px 24px rgba(15, 23, 42, 0.12)`
- Card text aligned center, so the title is centered

# Text blocks

- Title: `<h1>`, bold, margin 8px 0
- Description, profession, contact and keywords: left-aligned, margin 8px 0
- Contact: `<address>` with `font-style: normal`, 12px, plain text (not a link)

# Keywords

- Exactly 4 keywords in a `<ul>` (flex, wrap, gap 6px, no bullets) with `aria-label="Professional keywords"`
- Colors by position: `#1d4ed8`, `#b45309`, `#7e22ce`, `#be123c`
- Link: `href="https://duckduckgo.com/?q=<keyword without #>"`, `target="_blank"`, `rel="noopener noreferrer"`
- `aria-label="#<keyword>, search the web (opens in a new tab)"`
- Hover: `filter: brightness(55%)` plus a 1px underline
- Focus (links only): `outline: 2px solid #1D4ED8; outline-offset: 3px`
- Transition 160ms, disabled under `prefers-reduced-motion`

# Non-interactive elements

- Image, title, description and profession: no `tabindex`, no hover or focus styles, no `cursor: pointer`

# Content limits

- Description 20 words or fewer, profession 5 words or fewer
- Contact format: `name at domain` (no `@`)
- Keywords: `#` plus a single word, with a unique color each

# File output:

- Single html
- CSS in style tags
- Semantic HTML5
- Mobile reponsive
- ARIA accessibility
- Clean, commented code
- Output the raw HTML only: no markdown fences and no explanation
- Comment every CSS section and every HTML block
- No external files, fonts, scripts or images (the SVG is inline)

# Checks:

- an image should be rendered
- description should be no longer than 20 words
- profession should be no longer than five words
- contact information should have format: example at domain
- keywords should be separated and have different colors
- html is created
- css has style tags
- aria accessibility is present
