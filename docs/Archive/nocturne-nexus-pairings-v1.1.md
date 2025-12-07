# Nocturne Nexus Color Pairing Guide (v1.1)

This guide shows **recommended color pairings** on the main Nocturne Nexus backgrounds.
Version 1.1 aligns with the updated palette accent families and explicit accent caps.

Use this as a practical companion to the registry in `nocturne-nexus-palette-v1.1.md`.

---

## 1. Core backgrounds

These are the primary surfaces everything sits on:

- Core editor: `nn-bg-editor-core` = `#271E32`
- Panel / sidebar: `nn-bg-panel` = `#241B2F`
- Accent block / taskbar-like: `nn-bg-accent-block` = `#3E2E50`

---

## 2. Accent families (applied visually)

- **Primary-violet**  
  - Colors: `#B399FF`, `#A761EC`, `#C8A8FF`, `#FF80BF`, `#FF99D1`, `#B394D6`  
  - Use for: icons, logos, main interactive accents, syntax emphasis.

- **Secondary-warm**  
  - Colors: `#FFCA80`, `#FFDE9E`, `#FF9580`, `#FFB3A0`  
  - Use for: warnings, errors, and warm semantic emphasis only.

- **Tertiary-cool**  
  - Colors: `#80FFEA`, `#9AFFF0`  
  - Use for: cursor/caret, search highlight, tiny “electric” details.

- **Status-success**  
  - Colors: `#8AFF80`, `#A8FF9A`  
  - Use for: success/positive state only.

If you introduce new accents (for example, a teal variant), you must assign them to **one** of these families and document them in the palette registry.

---

## 3. Pairings for core backgrounds

These tables assume **dark UI** and are meant for icons, text, and borders.

### 3.1 Background: Core editor `#271E32` (`nn-bg-editor-core`)

| Element        | Recommended ID         | Hex       | Notes                                      |
|----------------|-----------------------|-----------|--------------------------------------------|
| Body text      | `nn-fg-primary`       | `#D8C5EE` | Main code / text                           |
| Secondary text | `nn-fg-muted`         | `#977DB5` | Comments, hints                            |
| Icon outline   | `nn-neutral-light`*   | `#B0B5C5` | Line icons, thin strokes                   |
| Icon fill      | `nn-accent-purple-primary` | `#B399FF` | Main glyph fill (primary-violet family)    |
| Accent detail  | `nn-accent-cyan-primary`   | `#80FFEA` | Tiny cool highlights, not whole icons      |
| Borders        | `nn-border-subtle`*   | `#3C3F46` | Card, panel, or icon container outlines    |

### 3.2 Background: Panel / sidebar `#241B2F` (`nn-bg-panel`)

| Element        | Recommended ID         | Hex       | Notes                                      |
|----------------|-----------------------|-----------|--------------------------------------------|
| Body text      | `nn-fg-primary`       | `#D8C5EE` | Main labels / navigation                   |
| Secondary text | `nn-fg-accent-soft`   | `#B394D6` | Inactive labels, low-priority info         |
| Icon outline   | `nn-neutral-light`*   | `#B0B5C5` | Readable but not overpowering              |
| Icon fill      | `nn-accent-purple-primary` | `#B399FF` | Primary sidebar icons                      |
| Accent detail  | `nn-accent-purple-glow`    | `#A761EC` | Inner glow / small highlights              |
| Borders        | `nn-border-subtle`*   | `#3C3F46` | Separators, edge lines                     |

### 3.3 Background: Accent block / taskbar `#3E2E50` (`nn-bg-accent-block`)

| Element        | Recommended ID         | Hex       | Notes                                      |
|----------------|-----------------------|-----------|--------------------------------------------|
| Body text      | `nn-fg-primary`       | `#D8C5EE` | Good contrast over `#3E2E50`               |
| Secondary text | `nn-fg-muted`         | `#977DB5` | Less prominent labels                      |
| Icon outline   | `nn-neutral-light`*   | `#B0B5C5` | Clear line icons on the taskbar            |
| Icon fill      | `nn-accent-purple-primary` | `#B399FF` | Main symbol color                          |
| Accent detail  | `nn-fg-bright`        | `#F5ECFF` | Tiny specular highlights / 3D shine        |
| Borders        | `nn-border-subtle`*   | `#3C3F46` | Optional, for separating taskbar segments  |

\* `nn-neutral-light` and `nn-border-subtle` are practical neutrals used for structure:
they are not in the original VS Code theme but are recommended utility colors for icons and borders.

Suggested values:

- `nn-neutral-light` = `#B0B5C5`  
- `nn-border-subtle` = `#3C3F46`  

If you adopt them, add them to the palette registry with appropriate metadata.

---

## 4. Quick decision rules

### 4.1 Surfaces

- Editor-like area → `nn-bg-editor-core` (`#271E32`)
- Sidebars & panels → `nn-bg-panel` (`#241B2F`)
- Taskbar / strong block → `nn-bg-accent-block` (`#3E2E50`)

### 4.2 Text

- High-readability text → `nn-fg-primary` (`#D8C5EE`)
- Hints/comments → `nn-fg-muted` (`#977DB5`)
- Low-priority labels → `nn-fg-accent-soft` (`#B394D6`)
- Sparing ultra-bright emphasis → `nn-fg-bright` (`#F5ECFF`)

### 4.3 Icons

On dark backgrounds:

- Outline / strokes → `nn-neutral-light` (`#B0B5C5`)
- Main fill → `nn-accent-purple-primary` (`#B399FF`)
- Tiny highlight → `nn-fg-bright` (`#F5ECFF`) or `nn-accent-cyan-primary` (`#80FFEA`)

### 4.4 Borders

- Default border/divider on dark surfaces → `nn-border-subtle` (`#3C3F46`)
- Only use colored borders (amber/green/red) when they carry **state meaning**.

---

## 5. Hard cap on accents (practical application)

To keep the interface balanced, apply a **hard cap** on how much visible area accents occupy,
following the well-known 60–30–10 guidance for color usage in UI:

- **~60%** of visible area: background family (`nn-bg-*`) and very dark structural elements.
- **~30%**: text (`nn-fg-*`) and neutral lines (`nn-border-subtle`, `nn-neutral-light`).  
- **≤10%**: all accents combined (`primary-violet`, `secondary-warm`, `tertiary-cool`, plus `status-success`).

Within that 10%:

- Most of the accent area should be **primary-violet** (brand purple/magenta).
- **Secondary-warm** appears mainly in warnings/errors and specific emphasis, not everywhere.
- **Tertiary-cool** should be a small fraction: cursor, search hits, small icon glows, not whole surfaces.

If your mockup starts looking “too colorful,” it usually means accent usage is creeping well above 10%.
Dial back cyan first, then warm accents, before touching the core purples.

---

## 6. When you are unsure what to pick

1. **If it’s a surface** → choose the nearest `nn-bg-*` that matches the depth (flat vs elevated vs strong block).

2. **If it’s text** → use `nn-fg-primary`, only downgrade to `nn-fg-muted` / `nn-fg-accent-soft` for secondary or disabled content.

3. **If it’s an icon** → outline = `nn-neutral-light`, fill = `nn-accent-purple-primary`.

4. **If it’s semantic (error/warn/success)** → pick from `nn-status-error*`, `nn-status-warning*`, `nn-status-success*`.

5. **If you catch yourself reaching for cyan for big shapes** → stop; that belongs in the tertiary family and should stay tiny.


When new colors are introduced for icons, wallpapers, or themes, they should be tested against these pairings:
does the new color cooperate with these background + text + icon combinations without fighting them? If not, the new color probably does not belong in Nocturne Nexus.
