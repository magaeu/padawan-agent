### `specs/contact-form-spec.md`

# Contact Form Specification

## Form content

- Render below the profile card
- Use a bordered box matching the existing card style
- Heading: `Contact Form`
- Fields:
  - Name: required
  - Email: required
  - Subject: required
  - Consent checkbox: required and unchecked by default
- Consent text: `I consent to the use of my information`
- Privacy-policy text: `Privacy Policy`
- Privacy-policy URL: `https://www.privacypolicytemplate.net/generic-privacy-policy/`
- Submit button text: `Submit`

## Fields

### Name

- Required
- Maximum 20 characters
- Trim leading and trailing whitespace
- Remove whitespace as specified by the submitted normalization rules
- Reject characters: `@#$%&*()!~?,<>/`

### Email

- Required
- Maximum 20 characters
- Trim leading and trailing whitespace
- Accept only the format `example@domain.com`

### Subject

- Required
- Maximum 180 characters
- Allow all characters
- Percent-encode characters `#$%&*()!~?,<>/` for submission state
- Display the original text to the user

### Consent

- Required
- Unchecked by default
- Show `This field is required` when unchecked

### Privacy Policy

- Render the text `Privacy Policy`
- Link to `https://www.privacypolicytemplate.net/generic-privacy-policy/`
- Open the link in a new tab

## Layout

- Place the form below the existing profile card
- Use a bordered box
- Match the profile card's border, spacing, radius, and text style
- Preserve a readable form width on mobile screens
- Align labels and fields consistently
- Keep the consent text and privacy link readable and grouped together

## Submission behavior

- This is a client-only demo
- Do not make a network or API request
- Trim and normalize Name and Email before validation
- Encode the Subject for submission state
- Keep the original Subject text visible
- Show the success view after valid submission
- Replace the form with:

```text
Your message was sent successfully. We will reach out soon!
```

- Clear all fields after successful submission
- Do not clear fields after validation errors
- There is no failure trigger in the successful client-only demo
- If a submission failure is introduced in the future, show:

```text
Your message could not be sent. Please try again later!
```

## Validation behavior

- Display field validation inline
- Use This field has an error. Please fix it before submit for field validation feedback
- Keep invalid fields and their entered values visible
- Mark the invalid fields and associated messages semantically
- Do not reveal implementation details or unsafe validation rules

## Feedback

**Success**

Replace the form with:

```text
Your message was sent successfully. We will reach out soon!
```

**Failure**

Reserve the following fallback:

```text
Your message could not be sent. Please try again later!
```

**Field validation**

Use:

```text
This field has an error. Please fix it before submit it.
```

Use `This field is required` for unchecked consent.

## Accessibility

- Use semantic form elements
- Associate every label with its corresponding control
- Mark required fields with HTML validation semantics
- Keep the consent checkbox keyboard accessible
- Add visible keyboard focus styles
- Render inline errors without removing the associated field values
- Announce validation and success feedback with live-region content
- Give the privacy-policy link an accessible name
- Add rel="noopener noreferrer" to the privacy-policy link

## Verification

- Confirm that the form appears below the profile card
- Confirm that Name, Email, and Subject are required
- Confirm that Name is limited to 20 characters
- Confirm that Name rejects @#$%&*()!~?,<>/
- Confirm that Name whitespace is trimmed
- Confirm that Email is limited to 20 characters
- Confirm that Email uses example@domain.com format
- Confirm that Email whitespace is trimmed
- Confirm that Subject is limited to 180 characters
- Confirm that specified Subject characters are encoded for submission state
- Confirm that the consent checkbox is required and unchecked initially
- Confirm that fields clear after success
- Confirm that fields remain populated after validation errors
- Confirm that success feedback replaces the form
- Confirm that inline validation and live-region feedback are present
- Confirm that the privacy-policy link opens in a new tab
- Confirm mobile layout and keyboard focus behavior
