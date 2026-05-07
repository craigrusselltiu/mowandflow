# Changelog

All notable changes to this project will be documented in this file. The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## v2.0.0 — 2026-05-07

### Changed

- Pivoted aesthetic direction to "Conservatory" dark luxury: deep forest greens, cream parchment typography, brass-gold accents used sparingly. Replaces the original warm off-white editorial-restraint direction.
- Hero is now full-bleed feel (~96vh) with text on the left and a portrait photograph on the right in a rounded frame with strong shadow and a subtle rotation.
- Services rebuilt as three lifted cards with rounded corners, soft shadows, brass numerals, hover lift, and a warm radial glow on hover.
- Gallery rebuilt as an irregular six-column grid with mixed-size photo cards.
- Approach restyled as a pull-quote moment with a brass curly quote, ampersand divider, and a faint giant italic ampersand watermark.
- Contact climax: lifted phone card with brass dot, massive Fraunces phone number, italic divider, and inline Instagram link.
- Updated `docs/SPEC.md` to reflect the new visual language; surfaces, shadows, gradients, and larger radii are now part of the system.

### Added

- Brass accent color `#D5B373` used for italic Fraunces emphasis, dots, hover states, and section numerals.
- Soft shadow and warm-glow tokens (`--shadow-md`, `--shadow-lg`, `--shadow-glow`).
- Animated brass scroll-tickle indicator below the hero.
- Subtle ambient radial halos behind the page and major sections.

### Removed

- Original tacky-feeling marquee strip.
- Floated drop cap in Approach.
- Two-column Contact layout (replaced by centered climax).
- Two-row Footer (collapsed to a single tight row).

## v1.0.0 — 2026-05-07

### Added

- Initial single-page site per `docs/SPEC.md`: header, hero, services, gallery, approach, service area, contact, footer.
- Wordmark with italic Fraunces ampersand at 1.15× scale.
- Sticky header that gains a hairline rule on scroll past the hero.
- Mobile nav: full-screen overlay with `aria-expanded` state and Escape-to-close.
- Hairline-only structural language.
- Placeholder image cards ready to be swapped for `<img>` tags.
- Favicon as a single SVG of the styled `&` glyph.
- GitHub Actions workflow at `.github/workflows/deploy.yml` for Pages deployment from `main`.
