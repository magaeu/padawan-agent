### `specs/footer-spec.md`

# Footer Specification

## Keywords

- Render exactly 4 keywords
- Use a `<ul>` element
- Set `aria-label="Professional keywords"`
- Use flex layout
- Allow wrapping
- Set `gap: 6px`
- Remove list bullets
- Each keyword must begin with `#`
- Each keyword must contain one word
- Assign each keyword a unique color
- Base keywords on the profile description and profession

## Keyword colors

Use these colors in order:

1. `#1d4ed8`
2. `#b45309`
3. `#7e22ce`
4. `#be123c`

## Keyword links

Each keyword must use:

- `href="https://duckduckgo.com/?q=<keyword without #>"`
- `target="_blank"`
- `rel="noopener noreferrer"`
- `aria-label="#<keyword>, search the web (opens in a new tab)"`

## Keyword interactions

On hover:

- Apply `filter: brightness(55%)`
- Add a 1px underline

For links in focus state:

- Apply `outline: 2px solid #1D4ED8`
- Apply `outline-offset: 3px`

Apply a `160ms` transition, but disable it under `prefers-reduced-motion`.

## Verification

- Confirm that an image is rendered
- Confirm that the description is no longer than 20 words
- Confirm that the profession is no longer than 5 words
- Confirm that contact uses `name at domain` format
- Confirm that 4 separated keywords have different colors
- Confirm that HTML is created
- Confirm that CSS is in style tags
- Confirm that ARIA attributes are present