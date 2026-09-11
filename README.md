# Multi-Step Checkout/Onboarding Form

A functional multi-step onboarding form built for the **"AI-Driven UI/UX Component Rapid Prototyping"** individual activity (Applied Generative AI for IT Solution Development, WPH Academy) — **Challenge B**.

## Overview

A 3-step onboarding flow (Profile → Company → Review) with:
- Step indicators showing active/completed state
- Per-field input validation with error messaging
- A success state on final submission
- Full keyboard accessibility and WCAG AA-compliant contrast

## Live Preview

https://dreadclamity.github.io/The-Multi-Step-Checkout-Onboarding-Form/

## Build Process

This prototype was generated and refined entirely through AI prompting across three iterations:

1. **Version 1** — Initial structural generation of the 3-step form.
2. **Version 2** — Fixed two structural flaws:
   - No responsive breakpoints (cramped step indicator on mobile)
   - Accessibility gaps (low text contrast, missing `aria-describedby`/`aria-invalid`, no focus management between steps)
3. **Version 3** — Fixed a critical interaction bug where pressing **Enter** on Step 1 triggered an implicit form submission via a hidden `type="submit"` button, skipping directly to the success state without completing Steps 2–3.

## Tech Stack

- HTML5
- CSS3 (custom properties, flexbox, media queries)
- Vanilla JavaScript (no frameworks/dependencies)

## Accessibility

- Text contrast verified at 5.66:1 (WCAG AA compliant)
- `aria-describedby` and `aria-invalid` wired to all validated inputs
- Programmatic focus management on every step transition
- Visible `:focus` states on all interactive elements

## License

No license added (educational/coursework project).
