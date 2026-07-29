# Maria Isabel Anda Varela Portfolio Design System

This site adapts the Aura Builder export into a senior HR portfolio visual language: premium, warm, practical, systems-minded, and human.

## Brand Feel

- Warm professional credibility, not a generic resume page.
- Senior HR portfolio meets proof-of-work page.
- Human organizational psychology layer with structured systems language.
- Dense enough to show substance, but broken into scannable cards.

## Colors

- Ink background: `#0C1208`
- Deep green background: `#141C0F`
- Cream surface: `#F0F4EC`
- Stone surface: `#DDE8D4`
- Accent green: `#4A8C2A`
- Accent lime: `#6DB33F`
- Dark text: `#111A0C`
- Light text: `#F4FAF0`
- Dark muted text: `#64745A`
- Light muted text: `#A8BA9C`

## Typography

- Headings: `Sora`, weights `500-800`
- Body: `Inter`, weights `400-800`
- Heading letter spacing: tight, usually `-0.055em` to `-0.085em`
- Body copy: generous line height, usually `1.7`
- Eyebrows: uppercase, high tracking, small size, green dot marker

## Layout

- Main content shell: `min(1240px, calc(100% - 2rem))`
- Navigation shell: `min(1440px, calc(100% - 2rem))`
- Section padding: about `7.5rem` desktop, `5.5rem` mobile
- Mobile-first behavior: all grids stack by `680px`, most complex layouts stack by `1000px`
- Alternate dark and light sections for rhythm and scannability
- Slanted section transitions may be used on major transitions only

## Components

### Header

- Fixed top navigation.
- Cream translucent background with blur.
- Name lockup with green gradient mark.
- Desktop shows anchor links.
- Mobile uses a simple accessible menu button.

### Buttons

- Primary: green/lime gradient, dark text, pill shape.
- Secondary: transparent glass treatment on dark sections, light surface on light sections.
- Text is uppercase with tracking for a confident technical feel.

### Cards

- Rounded corners: `20px` to `28px`.
- Light sections use white translucent surfaces and soft shadows.
- Dark sections use glass surfaces with subtle borders.
- Keep cards concise: headline, 1 short paragraph, optional tags or visual placeholder.

### Metrics

- Large `Sora` number or proof phrase.
- Short context below.
- Use for recruiter-scannable proof, not decoration.

### Accordions

- Use for detailed journey and long inventories.
- Default collapsed when the section could otherwise feel heavy.
- Content must still be useful when collapsed via strong summary labels.

### Visual Placeholders

- Use labeled placeholders until real public-safe visuals exist.
- Preferred future visuals: anonymized HR maps, workflow diagrams, dashboard mockups, culture check summaries, training visuals.
- Avoid generic corporate stock photos.

## Motion

- Current build avoids animation-heavy behavior for reliability.
- If motion is added later, use subtle fade/translate only.
- No parallax, no gimmicks, no distracting scroll effects.

## Accessibility

- High contrast between text and background.
- Buttons have clear descriptive labels.
- Accordions use native `details` and `summary`.
- Navigation uses semantic links and `aria` attributes.
- Avoid tiny text, especially on mobile.

## Content Rules

- Tone: clear, warm, confident, practical, human, direct.
- Avoid generic HR language and inflated leadership claims.
- Preserve the core positioning: senior HR professional, organizational psychologist, and People Operations professional who builds fair, practical, scalable People infrastructure.
- Use `Topax'` for possessive references if needed.
- Treat the resume PDF and case study visuals as follow-up assets until final files are ready.

## Adding New Pages

1. Create a new file in `src/pages/`, for example `src/pages/company-name.astro`.
2. Reuse `Header.astro`, `Footer.astro`, `SectionHeading.astro`, and the card classes in `global.css`.
3. Keep the same color rhythm: dark hero, light proof sections, dark closing CTA.
4. Add new reusable content to `src/data/` if it will be shared across pages.
5. Run `npm run build` before pushing.
