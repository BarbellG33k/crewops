# Crew Ops — Brand Color Palettes

> This file defines the approved brand color system for the Service Crew Pro website.
> Reference palette tokens by name when generating components, Tailwind configs, CSS custom properties, or design tokens.
> Each palette is self-contained and mutually exclusive — implement one at a time.

---

## Palette Overview

| # | Name | Background | Accent / CTA | Text | Secondary |
|---|------|------------|--------------|------|-----------|
| 1 | Rugged Charcoal & Safety Orange | `#1C1C1E` | `#FF6B00` | `#FFFFFF` / `#E4E4E7` | `#4A7C9B` |
| 2 | Blue Collar Classic | `#222D32` | `#F2B134` | `#F8F8F8` | `#35609A` |
| 3 | Modern Concrete & Signal Red | `#2E2E2E` | `#FF273A` | `#F0F1F3` | `#7EC3B6` |
| 4 | Grime & Shine | `#101418` | `#FDCB2E` | `#F5F5F7` | `#24527A` |
| 5 | Earned Respect | `#23303E` | `#FDB833` | `#F9F7F3` | `#A7A9AC` |

---

## Palette 1 — Rugged Charcoal & Safety Orange

**Personality:** Gritty, high-visibility, industrial authority. The safety orange commands action; charcoal grounds it with seriousness.

```css
:root {
  --color-bg:        #1C1C1E;
  --color-accent:    #FF6B00;
  --color-text:      #FFFFFF;
  --color-text-muted:#E4E4E7;
  --color-secondary: #4A7C9B;
}
```

| Role | Hex | Usage |
|------|-----|-------|
| Background | `#1C1C1E` | Page bg, card surfaces, nav |
| Accent / CTA | `#FF6B00` | Buttons, highlights, badges, links |
| Text Primary | `#FFFFFF` | Headlines, body copy |
| Text Muted | `#E4E4E7` | Subtext, captions, labels |
| Secondary | `#4A7C9B` | Secondary buttons, icons, dividers |

---

## Palette 2 — Blue Collar Classic

**Personality:** Trusted, seasoned, dependable. Gold signals quality and reward; deep navy-gray evokes a worn but respected work uniform.

```css
:root {
  --color-bg:        #222D32;
  --color-accent:    #F2B134;
  --color-text:      #F8F8F8;
  --color-text-muted:#F8F8F8cc;
  --color-secondary: #35609A;
}
```

| Role | Hex | Usage |
|------|-----|-------|
| Background | `#222D32` | Page bg, card surfaces, nav |
| Accent / CTA | `#F2B134` | Buttons, highlights, badges, links |
| Text Primary | `#F8F8F8` | Headlines, body copy |
| Text Muted | `#F8F8F8` at 80% opacity | Subtext, captions, labels |
| Secondary | `#35609A` | Secondary buttons, icons, dividers |

---

## Palette 3 — Modern Concrete & Signal Red

**Personality:** Urgent, bold, no-nonsense. Signal red stops the eye immediately; concrete gray keeps it from feeling alarming — more fast-paced job site than danger zone.

```css
:root {
  --color-bg:        #2E2E2E;
  --color-accent:    #FF273A;
  --color-text:      #F0F1F3;
  --color-text-muted:#F0F1F3cc;
  --color-secondary: #7EC3B6;
}
```

| Role | Hex | Usage |
|------|-----|-------|
| Background | `#2E2E2E` | Page bg, card surfaces, nav |
| Accent / CTA | `#FF273A` | Buttons, highlights, badges, links |
| Text Primary | `#F0F1F3` | Headlines, body copy |
| Text Muted | `#F0F1F3` at 80% opacity | Subtext, captions, labels |
| Secondary | `#7EC3B6` | Secondary buttons, icons, dividers |

---

## Palette 4 — Grime & Shine

**Personality:** Raw, underground, electric. Oil-black evokes the shop floor at midnight; electric yellow cuts through like a trouble light. High contrast, high energy.

```css
:root {
  --color-bg:        #101418;
  --color-accent:    #FDCB2E;
  --color-text:      #F5F5F7;
  --color-text-muted:#F5F5F7cc;
  --color-secondary: #24527A;
}
```

| Role | Hex | Usage |
|------|-----|-------|
| Background | `#101418` | Page bg, card surfaces, nav |
| Accent / CTA | `#FDCB2E` | Buttons, highlights, badges, links |
| Text Primary | `#F5F5F7` | Headlines, body copy |
| Text Muted | `#F5F5F7` at 80% opacity | Subtext, captions, labels |
| Secondary | `#24527A` | Secondary buttons, icons, dividers |

---

## Palette 5 — Earned Respect

**Personality:** Mature, approachable, professional. Workshop blue-gray reads as experienced rather than corporate; construction yellow signals momentum without aggression. Neutral gray softens the overall tone.

```css
:root {
  --color-bg:        #23303E;
  --color-accent:    #FDB833;
  --color-text:      #F9F7F3;
  --color-text-muted:#F9F7F3cc;
  --color-secondary: #A7A9AC;
}
```

| Role | Hex | Usage |
|------|-----|-------|
| Background | `#23303E` | Page bg, card surfaces, nav |
| Accent / CTA | `#FDB833` | Buttons, highlights, badges, links |
| Text Primary | `#F9F7F3` | Headlines, body copy |
| Text Muted | `#F9F7F3` at 80% opacity | Subtext, captions, labels |
| Secondary | `#A7A9AC` | Secondary buttons, icons, dividers |

---

## Implementation Guidance

### Tailwind CSS Config (v3)

Replace the hex values with whichever palette you select:

```js
// tailwind.config.js
module.exports = {
  theme: {
    extend: {
      colors: {
        'brand-bg':        'var(--color-bg)',
        'brand-accent':    'var(--color-accent)',
        'brand-text':      'var(--color-text)',
        'brand-muted':     'var(--color-text-muted)',
        'brand-secondary': 'var(--color-secondary)',
      },
    },
  },
}
```


