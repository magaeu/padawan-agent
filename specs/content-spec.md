### `specs/content-spec.md`

# Content Specification

## Profile content

- Profile description: 20 words or fewer
- Current profession: 5 words or fewer
- Contact information: email only
- Keywords: based on the description and profession
- Render description and profession in `<p>` elements
- Render contact in `<address>`

## Description

- Use a `<p>` element
- Left-align it
- Use `margin: 8px 0`
- Keep it to no more than 20 words
- Do not add `tabindex`
- Do not add hover or focus styles
- Do not use `cursor: pointer`

## Profession

- Use a `<p>` element
- Left-align it
- Use `margin: 8px 0`
- Keep it to no more than 5 words
- Do not add `tabindex`
- Do not add hover or focus styles
- Do not use `cursor: pointer`

## Contact

- Use `<address>`
- Display plain text without a link
- Set `font-style: normal`
- Set `font-size: 12px`
- Left-align it
- Use `margin: 8px 0`
- Use `name at domain` format
- Do not use `@`

Example:

```text
example at domain