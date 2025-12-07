# Nocturne Nexus Color Pairing Guide (v1.0)

This guide shows **recommended color pairings** on the main Nocturne Nexus backgrounds.

It’s a helper for choosing colors for **icons, borders, and text** without guessing.

---

## 1. Recommended base backgrounds

- Core editor: `#271E32`
- Panel / sidebar: `#241B2F`
- Accent block / taskbar-like: `#3E2E50`

---

## 2. Proposed new utility colors

These are *additions* to the main palette for structure and icon consistency.

| ID                | Hex       | Role                            | Typical usage                              |
|-------------------|----------|----------------------------------|--------------------------------------------|
| `nn-neutral-light`| `#B0B5C5`| Cool light neutral              | Icon strokes, neutral dividers, UI chrome  |
| `nn-border-subtle`| `#3C3F46`| Dark neutral border / outline   | Panel borders, card outlines on dark bg    |
| `nn-brand-primary`| `#B399FF`| Hero brand accent purple        | Logos, key glyphs, primary icon fills      |
| `nn-brand-surface`| `#3E2E50`| Brand-tinted surface / block    | Taskbar, selected blocks, “anchor” panels  |

`nn-brand-primary` and `nn-brand-surface` are aliases to colors already in the palette, promoted as explicit brand roles.

---

## 3. Pairings for core backgrounds

### 3.1 Background: Core editor `#271E32`

| Element        | Recommended color ID     | Hex       | Notes                                      |
|----------------|-------------------------|-----------|--------------------------------------------|
| Body text      | `nn-fg-primary`         | `#D8C5EE` | Main text                                  |
| Secondary text | `nn-fg-muted`           | `#977DB5` | Comments, hints                            |
| Icon outline   | `nn-neutral-light`      | `#B0B5C5` | Line icons, thin strokes                   |
| Icon fill      | `nn-brand-primary`      | `#B399FF` | Main glyph fill                            |
| Accent detail  | `nn-accent-cyan-primary`| `#80FFEA` | Small highlights, “techy” details          |
| Borders        | `nn-border-subtle`      | `#3C3F46` | Card, panel, or icon container outlines    |

### 3.2 Background: Panel / sidebar `#241B2F`

| Element        | Recommended color ID     | Hex       | Notes                                      |
|----------------|-------------------------|-----------|--------------------------------------------|
| Body text      | `nn-fg-primary`         | `#D8C5EE` | Same as editor                             |
| Secondary text | `nn-fg-accent-soft`     | `#B394D6` | Labels, inactive text                      |
| Icon outline   | `nn-neutral-light`      | `#B0B5C5` | Keeps icons legible but not screaming      |
| Icon fill      | `nn-brand-primary`      | `#B399FF` | Primary icon color                         |
| Accent detail  | `nn-accent-purple-glow` | `#A761EC` | Use sparingly as inner glow / highlight    |
| Borders        | `nn-border-subtle`      | `#3C3F46` | Separators, edge lines                     |

### 3.3 Background: Accent block / taskbar `#3E2E50`

| Element        | Recommended color ID     | Hex       | Notes                                      |
|----------------|-------------------------|-----------|--------------------------------------------|
| Body text      | `nn-fg-primary`         | `#D8C5EE` | Good contrast over 3E2E50                  |
| Secondary text | `nn-fg-muted`           | `#977DB5` | Less prominent labels                      |
| Icon outline   | `nn-neutral-light`      | `#B0B5C5` | Clear line icons on the taskbar            |
| Icon fill      | `nn-brand-primary`      | `#B399FF` | Main symbol color                          |
| Accent detail  | `nn-fg-bright`          | `#F5ECFF` | Tiny specular highlights / 3D shine        |
| Borders        | `nn-border-subtle`      | `#3C3F46` | Optional, for separating taskbar segments  |

---

## 4. Quick decision rules

1. **If it’s a surface**, start from:
   - `#271E32` (editor) → `nn-bg-editor-core`
   - `#241B2F` (sidebar) → `nn-bg-panel`
   - `#3E2E50` (strong block) → `nn-brand-surface`

2. **If it’s text on dark**, prefer:
   - Primary: `nn-fg-primary` (`#D8C5EE`)
   - Secondary: `nn-fg-muted` (`#977DB5`)

3. **If it’s a vector icon on dark**, use:
   - Outline: `nn-neutral-light` (`#B0B5C5`)
   - Fill: `nn-brand-primary` (`#B399FF`)
   - Tiny highlight: `nn-fg-bright` (`#F5ECFF`) or `nn-accent-cyan-primary` (`#80FFEA`)

4. **If you’re drawing a box around something**, default:
   - Border on dark backgrounds: `nn-border-subtle` (`#3C3F46`)

This keeps icons and borders consistent while still feeling like Nocturne Nexus.
