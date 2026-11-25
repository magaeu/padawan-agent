### `specs/style-spec.md`

# Style Specification

## Page

- Set page background to `#f3f4f6`
- Use `Arial, Helvetica, sans-serif`
- Set `body` margin to `0`
- Set `body` padding to `8px`
- Use CSS grid on `body`
- Set `place-items: center`
- Set `main` width to `100%`
- Use flex layout on `main`
- Center content in `main`

## Card

- Width: `400px`
- Maximum width: `calc(100% - 16px)`
- Margin: `8px`
- Padding: `8px`
- Border: `1px solid #e5e7eb`
- Top border: `4px solid #1D4ED8`
- Border radius: `12px`
- Box shadow: `0 8px 24px rgba(15, 23, 42, 0.12)`
- Align card text to the center
- Align the title to the center

## Text blocks

- Title:
  - `<h1>`
  - Bold
  - `margin: 8px 0`
- Description:
  - `<p>`
  - Left-aligned
  - `margin: 8px 0`
- Profession:
  - `<p>`
  - Left-aligned
  - `margin: 8px 0`
- Contact:
  - `<address>`
  - Left-aligned
  - `margin: 8px 0`
  - `font-style: normal`
  - `font-size: 12px`
- Keywords:
  - `<ul>`
  - Left-aligned
  - `margin: 8px 0`
  - Flex layout
  - Wrap items
  - Gap of `6px`
  - No bullets

## Accessibility

- Add appropriate ARIA attributes
- Use semantic HTML5 elements
- Keep non-interactive elements non-focusable
- Use the image's descriptive `aria-label`
- Use `aria-labelledby="profile-name"` on the article
- Use `aria-label="Professional keywords"` on the keyword list
- Add link-specific ARIA labels for the keywords
- Provide visible keyboard focus styles for links

## Responsive behavior

- Support mobile widths
- Restrict the card to `calc(100% - 16px)`
- Preserve the `400px` maximum width
- Allow keyword items to wrap

## Code requirements

- Produce one HTML file
- Place CSS in `<style>` tags
- Add clean comments
- Comment every CSS section
- Comment every HTML block
- Do not use external files
- Do not use external fonts
- Do not use scripts
- Do not use external images
- Keep the SVG inline
- Do not use `<img>`