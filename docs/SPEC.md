# Mow & Flow — Site Specification

A static single-page marketing site for Mow & Flow, a Sydney-based luxury lawn care and exterior home finishes business. Hosted on GitHub Pages.

## Brand

- **Name:** Mow & Flow
- **Tagline:** Clean execution. Consistent quality.
- **Voice:** Confident, restrained, editorial. No exclamation marks, no corporate-speak.
- **Audience:** Design-conscious Sydney homeowners.

## Logo (placeholder)

Wordmark: `MOW & FLOW` set in uppercase Fraunces, tight tracking. The `&` is rendered slightly larger (~1.18×) and in italic, in the brass accent color, to give it character. Placeholder pending a custom-drawn ampersand mark in a later iteration.

## Tech stack

- Plain HTML, CSS, JavaScript. No build step, no framework.
- Google Fonts: **Fraunces** (display, with `opsz` and `SOFT` axes), **Inter** (body).
- Vanilla JS for sticky-header state, mobile nav toggle, and small interactions.
- Hosted on GitHub Pages from `main` branch root via GitHub Actions.

## File structure

```
/
├── index.html
├── styles.css
├── main.js
├── favicon.svg
├── assets/                 (placeholder + Instagram-sourced images)
├── .github/workflows/      (Pages deployment)
├── docs/SPEC.md
├── README.md
└── CHANGELOG.md
```

## Visual design

### Direction — warm-parchment light luxury

Warm parchment foundation with cream-on-cream surfaces lifted by soft warm shadows. Deep warm-ink type as the dominant value. Antique-brass accent used sparingly for italic emphasis, dots, and hover. Green appears only inside photography (lawns, foliage) — never as a background or surface tint. Atmosphere comes from one warm-brass radial halo at the top of the page, italic Fraunces drama, and editorial section numbering.

Reference points: Aesop, Loewe, Le Labo, Apartamento, modern landscape-architect portfolios, editorial fashion-print on cream stock.

### Palette

| Token | Value | Use |
|---|---|---|
| `--bg` | `#F2ECD9` | Page background — warm parchment |
| `--bg-2` | `#EBE3C8` | Approach section, slightly deeper parchment |
| `--bg-card` | `#FBF7EA` | Card backgrounds (services, contact, photo cards) |
| `--bg-card-hover` | `#FFFCEF` | Card hover state |
| `--ink` | `#1F1A14` | Primary text — deep warm ink |
| `--ink-mid` | `#5C5043` | Body copy, secondary text |
| `--ink-soft` | `#8E8470` | Tertiary, eyebrow text |
| `--accent` | `#B8954F` | Antique brass for italic display, dots, hover, numbers |
| `--rule` | `rgba(31, 26, 20, 0.10)` | Hairlines |

Accent is used sparingly — italic Fraunces emphasis words, section numerals, dots, and hover states. Never as a fill on body text.

### Typography

- **Display:** Fraunces, weights 300–500, with `opsz` (9–144) and `SOFT` (0–100) variation axes used to adjust character at scale.
- **Body:** Inter, 300/400/500.
- **Scale:** Hero headline `clamp(56px, 7.4vw, 124px)`. Section titles `clamp(48px, 6vw, 96px)`. Contact phone `clamp(40px, 6.4vw, 96px)`.
- **Italic emphasis** in display copy uses the accent (`--accent`) color and a higher `SOFT` axis value for more curl.
- Line-height ~1.55 body, 0.94 display.

### Surface language

- **Shadows are allowed and encouraged** to create depth. Three shadow tokens: `--shadow-sm`, `--shadow-md`, `--shadow-lg`, plus a `--shadow-glow` (warm brass radial glow used on hover).
- **Radii:** cards use 16–24px, pills 999px. Larger radii are encouraged for tactility.
- **Subtle gradients** are allowed for ambient warmth (radial halos behind sections, hairline-like linear gradients on dividers, hover glow on cards). Heavy gradients on backgrounds are avoided.
- **Hairlines** remain a structural device, but rendered as low-opacity cream over the dark bg.
- **Card hover behavior:** translateY(-3..-4px) lift, shadow deepens, border picks up brass tint, soft warm radial glow appears.

### Layout principles

- Max content width 1320px; outer container with generous gutters.
- Vertical rhythm: clamp(96px, 12vw, 180px) between sections.
- Hero is full-bleed feel (~96vh) with a two-column grid: text on left, image on right.
- Asymmetric typography: progressive line indents in the hero headline.

## Site structure

Single page, anchor navigation, sections in order:

1. Header / nav
2. Hero
3. Services
4. Gallery
5. Approach
6. Service area
7. Contact
8. Footer

### 1. Header / nav

Sticky on scroll. Transparent over hero, gains a frosted backdrop and bottom rule when scrolled past 24px. Wordmark left, anchor links right. Mobile: hamburger expanding to full-viewport overlay menu with Fraunces serif items and hairline separators. Active link picks up brass color.

### 2. Hero

- Two-column grid, left: text; right: image.
- Eyebrow with brass italic numeral ("01"), gradient hairline, and label.
- Headline: `Clean / execution. / Consistent / quality.` with the italic words in brass and progressive indents.
- Subhead in muted parchment, max 38ch.
- Primary CTA: pill button with brass dot, "CALL" label, phone number in Fraunces, brass arrow on hover.
- Secondary CTA: underlined `See the work on Instagram →`.
- Image: portrait photograph in rounded 24px frame with strong soft shadow and a subtle 0.4° rotation that flips on hover. Caption below with brass `F.01` reference.
- Floating "SCROLL" indicator with animated brass tickle line.

### 3. Services

Three rounded, lifted cards on a subtle warm radial-halo background. Each card:

- Big italic Fraunces brass numeral (01, 02, 03) at top-left.
- Subtle arrow corner at top-right (animates on hover).
- Verb header in display Fraunces.
- Single-sentence description.
- Service list with brass `+` bullets, hairline separators, hover-shifts row right by 6px.
- Hover: card lifts, gains brass border tint and warm radial glow.

Verb groupings:

- **Maintain** — Lawn care, Garden maintenance
- **Clean** — Pressure washing, Gutter cleaning, Roof cleaning, Driveway cleaning
- **Build** — Driveway paving, Hardscaping

### 4. Gallery

Irregular grid (6 columns desktop) with mixed-size photo cards: one featured 4×2, one tall 2×2, one wide 4×1, plus standard 2×1. Each card has rounded corners, soft shadow, brass `G.0X` number top-left, and a small caption label bottom-left. Cards lift on hover. Real Instagram-sourced photos to replace placeholders progressively.

### 5. Approach

Pull-quote moment on slightly lighter forest bg, with a faint giant italic ampersand watermark drifting off the bottom-right.

- Centered, max-width 760px.
- Brass curly quote mark `"`.
- Italic Fraunces lede with brass emphasis on "deliberate, considered".
- Hairline divider with brass italic `&` in the center.
- Closing couplet — "Clean execution." / "Consistent quality." in display, second line in brass.
- "THAT'S THE WHOLE BRIEF." small-caps kicker.

### 6. Service area

Slim horizontal band: brass dot + `Servicing Sydney and surrounding suburbs — based in 2000.` Italic brass on "Sydney."

### 7. Contact

Centered hierarchy as the page's climax.

- "Get in touch." display headline with brass italic "touch."
- Lifted card containing brass dot + "CALL NOW" label and a massive `0404 845 845` in cream Fraunces. Card lifts and glows on hover.
- Italic "or" divider with hairlines on either side.
- Subtle inline link: `DM @mowandflow on Instagram →` with brass italic handle.
- Italic kicker: "For quotes, call or DM."

No form. No email.

### 8. Footer

Single tight row: wordmark left, meta links (phone · Instagram · Sydney NSW 2000) center, copyright right. Top hairline only. Hover on links picks up brass.

## Responsive behavior

- Primary breakpoint: 768px (mobile nav).
- Intermediate: 900–960px (hero stacks, services collapse to single column).
- All grids collapse cleanly. Photo card aspect ratios adjust per breakpoint.
- Type scales fluidly via `clamp()`.

## Accessibility

- Semantic HTML (`<header>`, `<main>`, `<section>`, `<footer>`, `<nav>`).
- All interactive elements keyboard-reachable with visible focus rings (brass `--accent` outline, 2px, with subtle radius).
- Color contrast: parchment cream `--ink` on deep forest `--bg` exceeds WCAG AA.
- Mobile nav state communicated via `aria-expanded`; Esc closes.
- `prefers-reduced-motion` respected — animations and the brass scroll-tickle disabled.

## Performance

- Inline critical CSS variables in `<head>` for first paint.
- `<link rel="preconnect">` for Google Fonts.
- Hero image uses `fetchpriority="high"`, `decoding="async"`, explicit `width`/`height` to reserve space.
- Other images `loading="lazy"`.
- Target: Lighthouse ≥ 95 on mobile.

## Favicon

Single SVG of the styled italic `&` glyph in `--accent` (brass) on `--bg` (deep forest). File: `favicon.svg`.

## Deployment

- Push to `main` branch of a public GitHub repo.
- Deploy via `.github/workflows/deploy.yml` to GitHub Pages (Actions source).
- Custom domain out of scope for v1.

## Out of scope for v1

- Custom-drawn ampersand mark (pending design)
- Real photography (placeholders until provided)
- Quote request form
- Map embed
- Blog / news section
- Analytics
