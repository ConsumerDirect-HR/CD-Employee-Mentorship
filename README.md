# ConsumerDirect Mentorship Program

A single-page site introducing ConsumerDirect's employee mentorship program: the **Orientation Buddy Program** (60-day onboarding pairing for new hires) and **ConsumerDirect Career Mentorship** (6-month goal-driven mentorship track), plus role-specific guidance and an FAQ.

## Structure

- `index.html` — the entire site (markup, styles, and navigation logic in one file, no build step)
- `logo.svg` — the ConsumerDirect logo used in the header

## Viewing locally

No build tools or server required — just open the file directly:

```
open index.html
```

## How it's organized

The page is a single HTML document with five sections toggled by the top nav (no page reloads, no routing library):

- **Home** — program overview and entry points into each track
- **Orientation Buddy Program** — the 60-day onboarding timeline
- **ConsumerDirect Career Mentorship** — the 6-month mentorship timeline
- **My Role** — tabbed guidance for New Hire / Orientation Buddy / Mentorship Participant / CD Career Mentor / Manager
- **FAQs** — expandable question list

Section/tab switching and FAQ toggles are handled by plain JavaScript (`showPage`, `showRole`, `toggleFaq`) at the bottom of `index.html`.

## Styling

- Font: [Nunito](https://fonts.google.com/specimen/Nunito) (loaded from Google Fonts)
- Colors are defined as CSS custom properties at the top of the `<style>` block in `index.html` (`--cd-blue`, `--cd-sky`, `--cd-orange`, `--cd-amber`, plus derived tints/shades), matching the brand colors in `logo.svg`

## Editing content

All copy lives directly in `index.html` under each section's `<div id="...">` block — there's no CMS or templating, so edits are just HTML changes.
