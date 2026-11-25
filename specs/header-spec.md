### `specs/header-spec.md`

# Header Specification

## Project

A profile card demonstrating build AI agents.

## Document structure

- Use `<!doctype html>`
- Set `<html lang="en">`
- Include `<meta charset="utf-8">`
- Include `<meta name="viewport" content="width=device-width, initial-scale=1">`
- Set the page title with `<title>`

Landmark order:

- `<main>`
  - `<article aria-labelledby="profile-name">`
    - Inline SVG
    - `<header>`
      - `<h1 id="profile-name">`

## Profile image

- Use an inline SVG, not `<img>`
- Set `viewBox="0 0 64 64"`
- Set width and height to `50`
- Display a developer figure with a `</>` laptop icon
- Do not include a `<title>` element
- Set `role="img"`
- Add a descriptive `aria-label`
- Center it with:
  - `display: block`
  - `margin: 8px auto`

## Title

- Render the title with `<h1>`
- Make it bold
- Use `margin: 8px 0`

## Non-interactive elements

The image and title must:

- Have no `tabindex`
- Have no hover or focus styles
- Not use `cursor: pointer`