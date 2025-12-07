# Nocturne Nexus Color Palette – Source of Truth (v1.0)

This document is the canonical color reference for **Nocturne Nexus**. 
All themes, icons, wallpapers, and logos should derive their colors from here.

There are two views:

1. **Machine-readable registry** – for AI and tooling (`id`, `hex`, roles).
2. **Human-oriented breakdown** – grouped by role with usage notes.

---

## 1. Machine-readable palette registry

Use this block as the single source of truth for automated systems or AI tools.

```jsonc
{
  "meta": {
    "paletteName": "Nocturne Nexus",
    "version": "1.0",
    "themeType": "dark",
    "source": "VS Code theme JSON (Nocturne-color-theme.json)",
    "author": "Lee Andrea + assistant"
  },
  "colors": [
    {
      "id": "nn-bg-panel",
      "hex": "#241B2F",
      "name": "Panel & Sidebar Background",
      "category": "background",
      "intent": "Secondary background for sidebars, panels, tabs, and controls.",
      "alphaVariants": [],
      "usageExamples": [
        "vscode.colors.sideBar.background",
        "vscode.colors.activityBar.background",
        "vscode.colors.panel.background",
        "vscode.colors.titleBar.activeBackground",
        "vscode.colors.tab.activeBackground",
        "vscode.colors.tab.inactiveBackground"
      ]
    },
    {
      "id": "nn-bg-elevated",
      "hex": "#261C31",
      "name": "Elevated Surface / Highlight Background",
      "category": "background",
      "intent": "Subtle elevated surfaces, line highlights, status bar background, selection frames.",
      "alphaVariants": [
        "#261C3180"
      ],
      "usageExamples": [
        "vscode.colors.panel.border",
        "vscode.colors.editor.inactiveSelectionBackground",
        "vscode.colors.editor.lineHighlightBackground",
        "vscode.colors.statusBar.background",
        "vscode.colors.statusBar.noFolderBackground",
        "vscode.colors.list.activeSelectionBackground"
      ]
    },
    {
      "id": "nn-bg-editor-core",
      "hex": "#271E32",
      "name": "Core Editor Background",
      "category": "background",
      "intent": "Primary dark canvas for code, terminals, and minimap.",
      "alphaVariants": [],
      "usageExamples": [
        "vscode.colors.editor.background",
        "vscode.colors.terminal.background",
        "vscode.colors.minimap.background",
        "vscode.colors.editorGutter.background"
      ]
    },
    {
      "id": "nn-bg-accent-block",
      "hex": "#3E2E50",
      "name": "Accent Block / Selection Background",
      "category": "background",
      "intent": "Stronger purple block used for selections, hovers, and high-emphasis surfaces.",
      "alphaVariants": [
        "#3E2E5040",
        "#3E2E5080"
      ],
      "usageExamples": [
        "vscode.colors.titleBar.inactiveBackground",
        "vscode.colors.tab.border",
        "vscode.colors.editor.selectionBackground",
        "vscode.colors.list.hoverBackground",
        "vscode.colors.dropdown.background",
        "vscode.colors.terminal.selectionBackground"
      ]
    },
    {
      "id": "nn-bg-scrollbar-track",
      "hex": "#49345E",
      "name": "Scrollbar Track & Rail",
      "category": "background",
      "intent": "Track / rail for scrollbars and narrow rails.",
      "alphaVariants": [
        "#49345E99",
        "#49345ECC",
        "#49345EFF"
      ],
      "usageExamples": [
        "vscode.colors.scrollbarSlider.background",
        "vscode.colors.scrollbarSlider.hoverBackground",
        "vscode.colors.scrollbarSlider.activeBackground"
      ]
    },
    {
      "id": "nn-accent-cyan-primary",
      "hex": "#80FFEA",
      "name": "Primary Cyan Accent",
      "category": "accent",
      "intent": "Cool accent for functions, info, and interactive badges.",
      "alphaVariants": [
        "#80FFEA15",
        "#80FFEA25",
        "#80FFEA40",
        "#80FFEA60",
        "#80FFEA80"
      ],
      "usageExamples": [
        "vscode.colors.badge.background",
        "vscode.colors.activityBarBadge.background",
        "vscode.colors.editorInfo.foreground",
        "vscode.colors.terminalCursor.foreground",
        "vscode.colors.terminal.ansiCyan",
        "vscode.colors.editor.findMatchBackground"
      ]
    },
    {
      "id": "nn-status-success",
      "hex": "#8AFF80",
      "name": "Success Green",
      "category": "status",
      "intent": "Success states, inserted/added code, and ANSI green.",
      "alphaVariants": [
        "#8AFF8015"
      ],
      "usageExamples": [
        "vscode.colors.diffEditor.insertedTextBackground",
        "vscode.colors.editorGutter.addedBackground",
        "vscode.colors.terminal.ansiGreen",
        "vscode.tokenColors.Strings (foreground)",
        "vscode.tokenColors.Inserted / Added (foreground)",
        "vscode.semanticTokenColors.string"
      ]
    },
    {
      "id": "nn-fg-muted",
      "hex": "#977DB5",
      "name": "Muted Text",
      "category": "foreground",
      "intent": "Comments, placeholders, and secondary labels.",
      "alphaVariants": [],
      "usageExamples": [
        "vscode.colors.titleBar.inactiveForeground",
        "vscode.colors.editorLineNumber.foreground",
        "vscode.colors.editorIndentGuide.activeBackground",
        "vscode.colors.input.placeholderForeground",
        "vscode.tokenColors.Comments (foreground)"
      ]
    },
    {
      "id": "nn-accent-cyan-bright",
      "hex": "#9AFFF0",
      "name": "Bright Cyan Accent",
      "category": "accent",
      "intent": "Bright cyan for ANSI bright cyan and very strong attention elements.",
      "alphaVariants": [],
      "usageExamples": [
        "vscode.colors.terminal.ansiBrightCyan"
      ]
    },
    {
      "id": "nn-accent-purple-glow",
      "hex": "#A761EC",
      "name": "Glow Purple Accent",
      "category": "accent",
      "intent": "High-energy purple for tab borders, active state glows, and logo details.",
      "alphaVariants": [],
      "usageExamples": [
        "vscode.colors.tab.activeBorderTop"
      ]
    },
    {
      "id": "nn-status-success-bright",
      "hex": "#A8FF9A",
      "name": "Bright Success Green",
      "category": "status",
      "intent": "Bright success or positive feedback in ANSI bright green.",
      "alphaVariants": [],
      "usageExamples": [
        "vscode.colors.terminal.ansiBrightGreen"
      ]
    },
    {
      "id": "nn-fg-accent-soft",
      "hex": "#B394D6",
      "name": "Soft Lavender Accent Text",
      "category": "foreground",
      "intent": "Subtle accent text, inactive tabs, and low-priority labels.",
      "alphaVariants": [],
      "usageExamples": [
        "vscode.colors.tab.inactiveForeground"
      ]
    },
    {
      "id": "nn-accent-purple-primary",
      "hex": "#B399FF",
      "name": "Primary Purple Accent",
      "category": "accent",
      "intent": "Core brand purple for buttons, property names, class names, and ANSI blue.",
      "alphaVariants": [],
      "usageExamples": [
        "vscode.colors.button.background",
        "vscode.colors.terminal.ansiBlue",
        "vscode.tokenColors.JSON Property Names / Object Keys (foreground)",
        "vscode.tokenColors.Classes, Types, Enums (foreground)",
        "vscode.tokenColors.Constants (foreground)",
        "vscode.tokenColors.Headings (foreground)"
      ]
    },
    {
      "id": "nn-accent-purple-bright",
      "hex": "#C8A8FF",
      "name": "Bright Purple Accent",
      "category": "accent",
      "intent": "Brightest purple for highlights and bright ANSI variants.",
      "alphaVariants": [],
      "usageExamples": [
        "vscode.colors.terminal.ansiBrightBlue"
      ]
    },
    {
      "id": "nn-fg-primary",
      "hex": "#D8C5EE",
      "name": "Primary Text",
      "category": "foreground",
      "intent": "Default text and high-readability foreground against dark backgrounds.",
      "alphaVariants": [],
      "usageExamples": [
        "vscode.colors.editor.foreground",
        "vscode.colors.sideBar.foreground",
        "vscode.colors.activityBar.foreground",
        "vscode.colors.titleBar.activeForeground",
        "vscode.colors.tab.activeForeground",
        "vscode.colors.editorLineNumber.activeForeground"
      ]
    },
    {
      "id": "nn-fg-bright",
      "hex": "#F5ECFF",
      "name": "Bright Accent Text",
      "category": "foreground",
      "intent": "Highest contrast light text used sparingly for strong emphasis.",
      "alphaVariants": [],
      "usageExamples": [
        "vscode.colors.terminal.ansiBrightWhite"
      ]
    },
    {
      "id": "nn-accent-magenta",
      "hex": "#FF80BF",
      "name": "Magenta Accent",
      "category": "accent",
      "intent": "Keywords, storage types, and ANSI magenta.",
      "alphaVariants": [],
      "usageExamples": [
        "vscode.colors.terminal.ansiMagenta",
        "vscode.tokenColors.Keywords & Storage (foreground)"
      ]
    },
    {
      "id": "nn-status-error",
      "hex": "#FF9580",
      "name": "Error Coral",
      "category": "status",
      "intent": "Errors, removed code, and ANSI red.",
      "alphaVariants": [
        "#FF958015",
        "#FF958040"
      ],
      "usageExamples": [
        "vscode.colors.diffEditor.removedTextBackground",
        "vscode.colors.editorError.foreground",
        "vscode.colors.editorGutter.deletedBackground",
        "vscode.colors.terminal.ansiRed",
        "vscode.colors.minimap.errorHighlight",
        "vscode.tokenColors.Error / Invalid (foreground)"
      ]
    },
    {
      "id": "nn-accent-magenta-bright",
      "hex": "#FF99D1",
      "name": "Bright Magenta Accent",
      "category": "accent",
      "intent": "ANSI bright magenta and ultra-vivid magenta highlights.",
      "alphaVariants": [],
      "usageExamples": [
        "vscode.colors.terminal.ansiBrightMagenta"
      ]
    },
    {
      "id": "nn-status-error-soft",
      "hex": "#FFB3A0",
      "name": "Soft Error Coral",
      "category": "status",
      "intent": "Softer error and ANSI bright red.",
      "alphaVariants": [],
      "usageExamples": [
        "vscode.colors.terminal.ansiBrightRed"
      ]
    },
    {
      "id": "nn-status-warning",
      "hex": "#FFCA80",
      "name": "Warning Amber",
      "category": "status",
      "intent": "Warnings, changed code, and ANSI yellow.",
      "alphaVariants": [
        "#FFCA8015",
        "#FFCA8030",
        "#FFCA8040"
      ],
      "usageExamples": [
        "vscode.colors.statusBar.debuggingBackground",
        "vscode.colors.editorWarning.foreground",
        "vscode.colors.editorGutter.modifiedBackground",
        "vscode.colors.terminal.ansiYellow",
        "vscode.colors.editor.wordHighlightBackground",
        "vscode.colors.editor.wordHighlightStrongBackground"
      ]
    },
    {
      "id": "nn-status-warning-bright",
      "hex": "#FFDE9E",
      "name": "Bright Warning Amber",
      "category": "status",
      "intent": "Loud warning and ANSI bright yellow.",
      "alphaVariants": [],
      "usageExamples": [
        "vscode.colors.terminal.ansiBrightYellow"
      ]
    }
  ]
}
```

---

## 2. Human-oriented breakdown

### 2.1 Core backgrounds

| ID | Hex | Name | Intended usage |
|---|-----|------|----------------|
| `nn-bg-panel` | `#241B2F` | Panel & Sidebar Background | Secondary background for sidebars, panels, tabs, and controls. |
| `nn-bg-elevated` | `#261C31` | Elevated Surface / Highlight Background | Subtle elevated surfaces, line highlights, status bar background, selection frames. |
| `nn-bg-editor-core` | `#271E32` | Core Editor Background | Primary dark canvas for code, terminals, and minimap. |
| `nn-bg-accent-block` | `#3E2E50` | Accent Block / Selection Background | Stronger purple block used for selections, hovers, and high-emphasis surfaces. |
| `nn-bg-scrollbar-track` | `#49345E` | Scrollbar Track & Rail | Track / rail for scrollbars and narrow rails. |

### 2.2 Text & foreground

| ID | Hex | Name | Intended usage |
|---|-----|------|----------------|
| `nn-fg-muted` | `#977DB5` | Muted Text | Comments, placeholders, and secondary labels. |
| `nn-fg-accent-soft` | `#B394D6` | Soft Lavender Accent Text | Subtle accent text, inactive tabs, and low-priority labels. |
| `nn-fg-primary` | `#D8C5EE` | Primary Text | Default text and high-readability foreground against dark backgrounds. |
| `nn-fg-bright` | `#F5ECFF` | Bright Accent Text | Highest contrast light text used sparingly for strong emphasis. |

### 2.3 Brand & accent colors

| ID | Hex | Name | Intended usage |
|---|-----|------|----------------|
| `nn-accent-cyan-primary` | `#80FFEA` | Primary Cyan Accent | Cool accent for functions, info, and interactive badges. |
| `nn-accent-cyan-bright` | `#9AFFF0` | Bright Cyan Accent | Bright cyan for ANSI bright cyan and very strong attention elements. |
| `nn-accent-purple-glow` | `#A761EC` | Glow Purple Accent | High-energy purple for tab borders, active state glows, and logo details. |
| `nn-accent-purple-primary` | `#B399FF` | Primary Purple Accent | Core brand purple for buttons, property names, class names, and ANSI blue. |
| `nn-accent-purple-bright` | `#C8A8FF` | Bright Purple Accent | Brightest purple for highlights and bright ANSI variants. |
| `nn-accent-magenta` | `#FF80BF` | Magenta Accent | Keywords, storage types, and ANSI magenta. |
| `nn-accent-magenta-bright` | `#FF99D1` | Bright Magenta Accent | ANSI bright magenta and ultra-vivid magenta highlights. |

### 2.4 Status & semantic colors

| ID | Hex | Name | Intended usage |
|---|-----|------|----------------|
| `nn-status-success` | `#8AFF80` | Success Green | Success states, inserted/added code, and ANSI green. |
| `nn-status-success-bright` | `#A8FF9A` | Bright Success Green | Bright success or positive feedback in ANSI bright green. |
| `nn-status-error` | `#FF9580` | Error Coral | Errors, removed code, and ANSI red. |
| `nn-status-error-soft` | `#FFB3A0` | Soft Error Coral | Softer error and ANSI bright red. |
| `nn-status-warning` | `#FFCA80` | Warning Amber | Warnings, changed code, and ANSI yellow. |
| `nn-status-warning-bright` | `#FFDE9E` | Bright Warning Amber | Loud warning and ANSI bright yellow. |

### 2.5 Alpha / overlay variants

These are **not separate base colors**. They are overlays derived from the base colors above.

| Base ID | Base Hex | Alpha variants (8‑digit hex) | Typical usage |
|---------|----------|------------------------------|---------------|
| `nn-bg-elevated` | `#261C31` | `#261C3180` | Hover / scrollbar / subtle background overlays |
| `nn-bg-accent-block` | `#3E2E50` | `#3E2E5040`, `#3E2E5080` | Hover / scrollbar / subtle background overlays |
| `nn-bg-scrollbar-track` | `#49345E` | `#49345E99`, `#49345ECC`, `#49345EFF` | Hover / scrollbar / subtle background overlays |
| `nn-accent-cyan-primary` | `#80FFEA` | `#80FFEA15`, `#80FFEA25`, `#80FFEA40`, `#80FFEA60`, `#80FFEA80` | Find / word highlights, diff overlays |
| `nn-status-success` | `#8AFF80` | `#8AFF8015` | Selection / highlight overlays |
| `nn-status-error` | `#FF9580` | `#FF958015`, `#FF958040` | Find / word highlights, diff overlays |
| `nn-status-warning` | `#FFCA80` | `#FFCA8015`, `#FFCA8030`, `#FFCA8040` | Find / word highlights, diff overlays |

---

## 3. Usage rules

High level rules for using this palette across assets:

1. **Background stacking**
   - Base: `nn-bg-editor-core` (`#271E32`).
   - Slightly raised surfaces: `nn-bg-elevated` (`#261C31`).
   - Sidebars / panels / chrome: `nn-bg-panel` (`#241B2F`).
   - Heavy blocks / taskbar-like bars: `nn-bg-accent-block` (`#3E2E50`).

2. **Text hierarchy**
   - Primary body text: `nn-fg-primary` (`#D8C5EE`).
   - Muted / comments / placeholders: `nn-fg-muted` (`#977DB5`).
   - Soft accent labels (inactive tab labels, low-importance text): `nn-fg-accent-soft` (`#B394D6`).
   - Rare, strongest emphasis (small doses): `nn-fg-bright` (`#F5ECFF`).

3. **Brand accent strategy**
   - Primary brand accent: `nn-accent-purple-primary` (`#B399FF`).
   - Glow / energy: `nn-accent-purple-glow` (`#A761EC`).
   - Brightest purple (sparingly): `nn-accent-purple-bright` (`#C8A8FF`).
   - Cool accent / tech feel: `nn-accent-cyan-primary` (`#80FFEA`).
   - Ultra-bright cyan: `nn-accent-cyan-bright` (`#9AFFF0`) for ANSI and very strong highlights.

4. **Status / feedback colors**
   - Success: `nn-status-success` (`#8AFF80`) and bright variant `nn-status-success-bright` (`#A8FF9A`).
   - Warning: `nn-status-warning` (`#FFCA80`) and bright variant `nn-status-warning-bright` (`#FFDE9E`).
   - Error: `nn-status-error` (`#FF9580`) and softer variant `nn-status-error-soft` (`#FFB3A0`).
   - Magenta accents: `nn-accent-magenta` (`#FF80BF`) / `nn-accent-magenta-bright` (`#FF99D1`) mainly for keywords and ANSI magenta.

5. **Overlays & interaction states**
   - Use alpha variants based on the same base color instead of inventing new semi-random hex values.
   - Selections / highlights should stay within the `nn-bg-*` or `nn-accent-cyan-primary` / `nn-status-warning` / `nn-status-error` families.

---

## 4. How to extend the palette

When adding a **new color** (for icons, wallpaper, logos, or new themes):

1. **Decide if a new color is really needed**
   - If you can express it as an alpha variant or reuse an existing accent, prefer that.

2. **If a new color is required**
   - Pick a hex that visually sits in the Nocturne Nexus family (dark violet / neon cyan / coral / amber).
   - Add a new entry to the JSON registry in section 1 with:
     - `id` following the pattern: `nn-<category>-<short-name>`.
     - `hex` with uppercase hex digits.
     - `category` ∈ {`background`, `foreground`, `accent`, `status`} (or a new category if justified).
     - `intent` explaining *why* it exists.
     - `alphaVariants` if you immediately know the overlay variants you will use.
     - `usageExamples` listing where it is used (e.g. `"icons.terminal.3dFace"`).

3. **Update cross-references**
   - If the color is used in VS Code, add the relevant `vscode.*` entries in `usageExamples`.
   - For other assets (icons, wallpapers, branding), use namespaced strings such as:
     - `icons.vscode.logoPrimary`
     - `wallpaper.orbitalSyntax.nodeHighlight`
     - `operaGX.themeAccent.primary`

---

## 5. Known gaps / open slots

Based on the current VS Code theme, the palette is already consistent. 
However, for future icons and wallpapers there are a few **intentional gaps** you may want to fill later:

1. **Stroke / outline neutral**
   - There is no dedicated thin-outline color distinct from `nn-bg-elevated` / `nn-bg-accent-block`.
   - For SVG icon outlines and borders, you may want a slightly lighter, cool outline (e.g. a desaturated violet).

2. **Grayscale-neutral option**
   - Everything is tinted purple/cyan/orange. If you ever need a true neutral gray, it should be added explicitly as `nn-fg-neutral` rather than improvised.

3. **Logo-first primary purple**
   - `nn-accent-purple-primary` (`#B399FF`) works for now, but if logo design needs a more saturated or slightly darker hero purple, promote it into its own `nn-brand-primary` entry.

4. **Depth ramp for 3D icons**
   - 3D icons often benefit from 3–4 steps of the same hue (shadow / mid / light / highlight).
   - Right now, the dark purples work, but you may want a defined ramp like:
     - `nn-3d-purple-shadow`
     - `nn-3d-purple-mid`
     - `nn-3d-purple-light`
     - `nn-3d-purple-highlight`
   - Those would still live inside the purple family but be tuned for shading.

When any of these gaps are filled, **this document must be updated first**, and all downstream assets should treat it as the authority.
