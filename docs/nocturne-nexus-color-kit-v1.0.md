# Nocturne Nexus · Color System & Figma Color Kit (v1.0)

## 1. Theme summary

- Theme type: Dark
- Core editor background: `#271E32`
- Core panel / chrome background: `#241B2F`
- Primary text on dark surfaces: `#D8C5EE`
- Muted text: `#977DB5`
- Primary accent: `#B399FF` (lavender)
- Secondary accents: `#80FFEA` (aqua), `#8AFF80` (green), `#FFCA80` (amber), `#FF80BF` / `#FF99D1` (pinks)
- Semantic: error `#FF9580`, warning `#FFCA80`, success `#8AFF80`

This document extracts a structured color system from the Nocturne Nexus VS Code theme and aligns it with the Aurora kit.

---

## 2. Core palette

### 2.1 Surface colors

| Figma style name             | Hex       | VS Code tokens (examples)                                    | Role                         |
|-----------------------------|-----------|--------------------------------------------------------------|------------------------------|
| NN / Bg / Editor Core       | `#271E32` | `editor.background`, `terminal.background`, `minimap.background`, `editorGutter.background` | Main canvas / code           |
| NN / Bg / Panel             | `#241B2F` | `panel.background`, `sideBar.background`, `activityBar.background`, `titleBar.activeBackground` | Panels, sidebar, main chrome |
| NN / Bg / Panel Alt         | `#261C31` | `statusBar.background`, `list.activeSelectionBackground`, `list.focusBackground`, `editor.lineHighlightBackground` | Slightly raised surfaces     |
| NN / Bg / Border Hard       | `#3E2E50` | `panel.border`, `tab.border`, `titleBar.inactiveBackground`, `sideBar.border`, `border`, minimap overlays | Hard separators              |
| NN / Bg / Scroll Track      | `#241B2F` | implied                                                     | Scrollbar track              |
| NN / Bg / Scroll Slider     | `#49345E` | scrollbar slider backgrounds (with varying alpha)            | Scroll handle                |

### 2.2 Text & foreground

| Figma style name          | Hex       | VS Code tokens (examples)                       | Role                          |
|---------------------------|-----------|------------------------------------------------|-------------------------------|
| NN / Text / Primary       | `#D8C5EE` | `editor.foreground`, `sideBar.foreground`, `activityBar.foreground`, `titleBar.activeForeground` | Primary text on dark surfaces |
| NN / Text / Muted         | `#977DB5` | comments, inactive titles, line numbers        | Secondary / muted text        |
| NN / Text / Inactive Tab  | `#B394D6` | `tab.inactiveForeground`                       | Inactive tabs                 |
| NN / LineNumber / Base    | `#977DB5` | `editorLineNumber.foreground`                  | Gutter line numbers           |
| NN / LineNumber / Active  | `#D8C5EE` | `editorLineNumber.activeForeground`            | Active line number            |
| NN / Cursor               | `#D8C5EE` | `editorCursor.foreground`                      | Editor cursor                 |
| NN / Placeholder          | `#977DB5` | `input.placeholderForeground`                  | Input placeholders            |

### 2.3 Accent & syntax colors

| Figma style name             | Hex       | VS Code usage                                   |
|-----------------------------|-----------|------------------------------------------------|
| NN / Accent / Lavender      | `#B399FF` | JSON keys, classes, headings, constants        |
| NN / Accent / Aqua          | `#80FFEA` | functions, methods, info, links, cursor        |
| NN / Accent / Green         | `#8AFF80` | strings, inserted markup                       |
| NN / Accent / Amber         | `#FFCA80` | numbers, booleans, warnings, changed markup    |
| NN / Accent / Pink          | `#FF80BF` | keywords, storage                              |
| NN / Accent / Pink Soft     | `#FF99D1` | bright magenta / emphasis                      |
| NN / Accent / Lavender Soft | `#C8A8FF` | bright blue, softer lavender                   |
| NN / Accent / Orange Soft   | `#FFDE9E` | bright yellow                                  |
| NN / Accent / Orange Strong | `#FFB3A0` | bright red                                     |

### 2.4 Semantic colors

| Figma style name          | Hex       | VS Code usage                       |
|--------------------------|-----------|-------------------------------------|
| NN / Semantic / Error    | `#FF9580` | `editorError.foreground`, removed   |
| NN / Semantic / Warning  | `#FFCA80` | `editorWarning.foreground`, changed |
| NN / Semantic / Info     | `#80FFEA` | `editorInfo.foreground`             |
| NN / Semantic / Success  | `#8AFF80` | added resources                     |

Translucent overlays to mirror VS Code 8‑digit hex:

- `NN / Overlay / Selection` → `#3E2E5080`
- `NN / Overlay / Word` → `#FFCA8015`
- `NN / Overlay / Word Strong` → `#FFCA8030`
- `NN / Overlay / Find` → `#80FFEA40`
- `NN / Overlay / Find Soft` → `#80FFEA25`
- `NN / Overlay / Find Range` → `#80FFEA15`
- `NN / Overlay / Fold` → `#261C3180`
- `NN / Overlay / Bracket` → `#3E2E5040`

---

## 3. Recommended pairings

### 3.1 Core editor

- **Base editor**
  - Bg: `NN / Bg / Editor Core` (`#271E32`)
  - Text: `NN / Text / Primary`
  - Muted: `NN / Text / Muted`
  - Accent: `NN / Accent / Lavender` and `NN / Accent / Aqua`

- **Line highlight**
  - Bg: `NN / Bg / Panel Alt` (`#261C31`) or `NN / Overlay / Selection` overlay as desired.

### 3.2 Sidebar / panel / title bar

- **Sidebar**
  - Bg: `NN / Bg / Panel`
  - Text: `NN / Text / Primary`
  - Muted: `NN / Text / Muted`

- **Bottom panel (Problems / Output / Terminal)**
  - Bg: `NN / Bg / Panel`
  - Border: `NN / Bg / Border Hard`
  - Text: `NN / Text / Primary` / `NN / Text / Muted`
  - Accent: `NN / Accent / Lavender` for active tab underline.

- **Title bar**
  - Active bg: `NN / Bg / Panel`
  - Inactive bg: `NN / Bg / Border Hard`
  - Active text: `NN / Text / Primary`
  - Inactive text: `NN / Text / Muted`

### 3.3 Terminal

- Bg: `NN / Bg / Editor Core`
- Text: `NN / Text / Primary`
- Cursor: `NN / Accent / Aqua`
- ANSI mapping is already defined in the theme:
  - Green: `NN / Accent / Green`
  - Yellow: `NN / Accent / Amber`
  - Blue: `NN / Accent / Lavender`
  - Magenta: `NN / Accent / Pink`
  - Cyan: `NN / Accent / Aqua`
  - Bright variants use softer tints (`NN / Accent / Lavender Soft`, etc.).

### 3.4 Notifications / callouts

- Info: bg `NN / Bg / Panel Alt`, border `NN / Accent / Aqua`
- Warning: bg `NN / Bg / Panel Alt`, border `NN / Semantic / Warning`
- Error: bg `NN / Bg / Panel Alt`, border `NN / Semantic / Error`

---

## 4. Figma Color Kit structure

### 4.1 Pages

Mirror Aurora’s structure but with `NN` prefixing styles:

1. `01 · Nocturne / Palette`
2. `02 · Nocturne / UI Frames`
3. `03 · Nocturne / Code Samples`
4. `04 · Nocturne / Tokens (Tokens Studio)`

### 4.2 Swatch frames (Page 01)

Use the same grouping pattern as Aurora:

- `Bg · Core`
- `Text · Core`
- `Accent · Core`
- `Semantic · Core`
- `Overlays`

Example swatches:

- `NN / Bg / Editor Core` → `#271E32`
- `NN / Bg / Panel` → `#241B2F`
- `NN / Bg / Panel Alt` → `#261C31`
- `NN / Text / Primary` → `#D8C5EE`
- `NN / Accent / Lavender` → `#B399FF`
- `NN / Accent / Aqua` → `#80FFEA`
- `NN / Semantic / Error` → `#FF9580`

Each swatch uses the same two-line label pattern:

1. Line 1: style name
2. Line 2: hex value

### 4.3 UI frames (Page 02)

Reuse your existing Nocturne frames if you already have them (`Nocturne Nebula`, `Orbital Syntax` mini‑comps). Ensure they pull styles from the new names above instead of hardcoded fills.

Suggested frames:

- `NN · Editor Frame`
- `NN · Sidebar + Panel`
- `NN · Terminal`
- `NN · Notification Stack`

### 4.4 Tokens Studio setup (Page 04)

Token sets to parallel Aurora:

- `nocturne/core/bg`
- `nocturne/core/text`
- `nocturne/core/accent`
- `nocturne/semantic`
- `nocturne/overlay`

Example tokens:

- `nocturne.core.bg.editor` → `#271E32`
- `nocturne.core.bg.panel` → `#241B2F`
- `nocturne.core.bg.panelAlt` → `#261C31`
- `nocturne.core.text.primary` → `#D8C5EE`
- `nocturne.accent.lavender` → `#B399FF`
- `nocturne.semantic.error` → `#FF9580`

This keeps Aurora and Nocturne structurally identical from a token perspective, which makes maintaining the two VS Code themes and any future apps less painful.
