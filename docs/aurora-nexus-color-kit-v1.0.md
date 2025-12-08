# Aurora Nexus · Color System & Figma Color Kit (v1.0)

## 1. Theme summary

- Theme type: Light
- Core editor background: `#E4D8FB`
- Core panel / chrome background: `#D7C6F7`
- Primary text on light surfaces: `#241B2F`
- Muted text: `#6D5B98`
- Primary accent: `#B399FF` (lavender)
- Secondary accents: `#A761EC` (indigo), `#80FFEA` / `#33B9A6` (aqua / teal), `#FF9A3C` / `#FF80BF` / `#FF99D1` (warm & pinks)
- Semantic: error `#FF9580`, warning `#FF9A3C`, success `#33B9A6`

This document turns the Aurora Nexus VS Code theme into a reusable color system and Figma Color Kit.

---

## 2. Core palette

### 2.1 Surface colors

| Figma style name           | Hex       | VS Code tokens (examples)                            | Role                          |
|---------------------------|-----------|------------------------------------------------------|-------------------------------|
| AN / Bg / Editor Core     | `#E4D8FB` | `editor.background`, `minimap.background`           | Main canvas / editor          |
| AN / Bg / Panel           | `#D7C6F7` | `panel.background`, `activityBar.background`, `statusBar.background`, `editorGroupHeader.*`, `tab.activeBackground` | Panels, chrome, active tabs   |
| AN / Bg / Sidebar         | `#E4D8FB` | `sideBar.background`                                | Sidebar body                  |
| AN / Bg / Sidebar Header  | `#D7C6F7` | `sideBarSectionHeader.background`                   | Sidebar section headers       |
| AN / Bg / Elevated        | `#ECE2FF` | `tab.hoverBackground`, `list.focusBackground`, `list.hoverBackground`, `notifications.background`, `dropdown.background` | Hover / focused surfaces      |
| AN / Bg / Input           | `#F5ECFF` | `input.background`, `peekViewEditor.background`     | Inputs, inline editors        |
| AN / Bg / Subtle Border   | `#C6B7E5` | `border`, `sideBar.border`, `panel.border`, `tab.border`, `dropdown.border`, `input.border`, `editorRuler.foreground` | Neutral borders / rulers      |
| AN / Bg / Indent Guide    | `#D9CFF0` | `editorIndentGuide.background`                      | Indent guides (inactive)      |
| AN / Bg / Indent Active   | `#B399FF` | `editorIndentGuide.activeBackground`                | Active indent guide           |
| AN / Bg / Gutter          | `#E4D8FB` | `editorGutter.background`                           | Gutter background             |
| AN / Bg / Scroll Track    | `#E4D8FB` | implicit                                            | Scroll track base             |
| AN / Bg / Minimap Slider  | `#D7C6F7` | `minimapSlider.background`                          | Minimap viewport              |
| AN / Bg / Minimap Slider Hover | `#C8A8FF` | `minimapSlider.hoverBackground`               | Minimap slider hover          |
| AN / Bg / Minimap Slider Active | `#B399FF` | `minimapSlider.activeBackground`               | Minimap slider active         |

### 2.2 Text & foreground

| Figma style name        | Hex       | VS Code tokens (examples)                                   | Role                          |
|-------------------------|-----------|-------------------------------------------------------------|-------------------------------|
| AN / Text / Primary     | `#241B2F` | `foreground`, `variable`, `panelTitle.activeForeground`, `titleBar.activeForeground` | Primary text on light surfaces |
| AN / Text / Muted       | `#6D5B98` | `sideBar.foreground`, inactive tabs, placeholders          | Secondary / muted text        |
| AN / Text / Accent      | `#B399FF` | headings, badges, buttons                                  | Emphasis text                 |
| AN / Text / Inverted    | `#E4D8FB` | for rare use on very dark custom surfaces                  | Text on dark chips / badges   |
| AN / LineNumber / Base  | `#6D5B98` | `editorLineNumber.foreground`                              | Gutter line numbers (resting) |
| AN / LineNumber / Active| `#C5A8F7` | `editorLineNumber.activeForeground`                        | Active line number            |
| AN / Cursor             | `#80FFEA` | `editorCursor.foreground`, `terminalCursor.foreground`     | Editor & terminal cursor      |
| AN / Placeholder        | `#6D5B98` | `input.placeholderForeground`                              | Placeholder text              |

### 2.3 Accent & syntax colors

| Figma style name            | Hex       | VS Code usage                                      |
|----------------------------|-----------|---------------------------------------------------|
| AN / Accent / Lavender     | `#B399FF` | functions, tags, badges, active borders           |
| AN / Accent / Lavender Soft| `#C8A8FF` | `button.hoverBackground`, minimap slider hover    |
| AN / Accent / Indigo       | `#A761EC` | classes / types                                   |
| AN / Accent / Aqua         | `#80FFEA` | cursor, word highlights, focus accents            |
| AN / Accent / Teal         | `#33B9A6` | numbers, some terminal cyan, VCS added            |
| AN / Accent / Warm Orange  | `#FF9A3C` | strings, property.readonly, VCS modified          |
| AN / Accent / Pink         | `#FF80BF` | keywords / storage                                |
| AN / Accent / Pink Soft    | `#FF99D1` | constants                                         |
| AN / Accent / Deep Plum    | `#4A3C65` | punctuation, parameters                           |
| AN / Accent / Cyan Bright  | `#52C7B8` | `terminal.ansiBrightCyan`                         |

### 2.4 Semantic colors

| Figma style name           | Hex       | VS Code usage                        |
|---------------------------|-----------|--------------------------------------|
| AN / Semantic / Error     | `#FF9580` | invalid tokens, deleted resources    |
| AN / Semantic / Warning   | `#FF9A3C` | modified VCS resources               |
| AN / Semantic / Success   | `#33B9A6` | added / untracked VCS resources      |
| AN / Semantic / Info      | `#80FFEA` | cursor, some highlights              |

For translucency tokens (selection, highlights, etc.), define them in Figma as separate styles using 8‑digit hex or opacity overlays:

- `AN / Overlay / Selection` → `#D7C6F733`
- `AN / Overlay / Selection Inactive` → `#D7C6F722`
- `AN / Overlay / Selection Highlight` → `#FF9A3C30`
- `AN / Overlay / Word Highlight` → `#80FFEA22`
- `AN / Overlay / Word Strong` → `#80FFEA33`
- `AN / Overlay / Bracket` → `#B399FF22`

---

## 3. Recommended pairings

These are ready-made combinations for UI and marketing work.

### 3.1 Code editor

- **Base editor**
  - Bg: `AN / Bg / Editor Core` (`#E4D8FB`)
  - Text: `AN / Text / Primary` (`#241B2F`)
  - Muted: `AN / Text / Muted` (`#6D5B98`)
  - Accent: `AN / Accent / Lavender`
- **Line focus**
  - Keep `editor.lineHighlightBackground` visually subtle by using `AN / Overlay / Selection Inactive` as a basis if you want more contrast than the current flat background.

### 3.2 Panels & sidebars

- **Primary panel (Problems / Output / Terminal)**
  - Bg: `AN / Bg / Panel`
  - Text: `AN / Text / Primary` for active, `AN / Text / Muted` for inactive
  - Border: `AN / Bg / Subtle Border`
  - Accent: `AN / Accent / Lavender` for active tab / underline

- **Sidebar**
  - Bg: `AN / Bg / Sidebar`
  - Section header bg: `AN / Bg / Sidebar Header`
  - Icons: use `AN / Text / Muted` for inactive, `AN / Accent / Lavender` for active.

### 3.3 Callouts / notifications

- Info: bg `AN / Bg / Elevated`, border `AN / Accent / Aqua`, text `AN / Text / Primary`.
- Warning: bg `AN / Bg / Elevated`, border `AN / Semantic / Warning`, accent icons same.
- Error: bg `AN / Bg / Elevated`, border `AN / Semantic / Error`.

### 3.4 Terminal

- Bg: `AN / Bg / Editor Core` (`terminal.background`)
- Text: `AN / Text / Muted`
- Cursor: `AN / Accent / Aqua`
- Accent mapping:
  - Cyan: `AN / Accent / Teal` / `AN / Accent / Cyan Bright`
  - Use pinks and oranges sparingly since strings and keywords already sit in that range in the editor.

---

## 4. Figma Color Kit structure

### 4.1 Pages

Use the same page structure as Nocturne, with Aurora-specific styles:

1. `01 · Aurora / Palette`
2. `02 · Aurora / UI Frames`
3. `03 · Aurora / Code Samples`
4. `04 · Aurora / Tokens (Tokens Studio)`

### 4.2 Swatch frames (Page 01)

Create frames:

- `Bg · Core`
- `Text · Core`
- `Accent · Core`
- `Semantic · Core`
- `Overlays`

Inside each frame, create rectangles with the style names listed above, e.g.:

- `AN / Bg / Editor Core`
- `AN / Bg / Panel`
- `AN / Text / Primary`
- `AN / Accent / Lavender`
- etc.

Put a text layer at the bottom of each swatch with:

1. Line 1: style name (e.g. `AN / Bg / Panel`)
2. Line 2: hex value (e.g. `#D7C6F7`)

### 4.3 UI frames (Page 02)

Create “mini‑comps” that mirror VS Code layouts:

- **AN · Editor Frame**
  - Use `AN / Bg / Editor Core` for background.
  - Code block using syntax colors.
- **AN · Sidebar + Panel Frame**
  - Left sidebar using `AN / Bg / Sidebar` etc.
  - Bottom panel using `AN / Bg / Panel` and panel text styles.
- **AN · Terminal Frame**
  - Terminal block using the terminal palette subset.

Use these to visually QA changes when you tweak colors.

### 4.4 Tokens Studio setup (Page 04)

Suggested token sets:

- `aurora/core/bg`
- `aurora/core/text`
- `aurora/core/accent`
- `aurora/semantic`
- `aurora/overlay`

Example tokens:

- `aurora.core.bg.editor` → `#E4D8FB`
- `aurora.core.bg.panel` → `#D7C6F7`
- `aurora.core.text.primary` → `#241B2F`
- `aurora.accent.lavender` → `#B399FF`
- `aurora.semantic.error` → `#FF9580`

Map Figma styles to tokens using the same naming fragments (`bg.editor`, `text.primary`, etc.) so you can keep Aurora and Nocturne aligned structurally while differing in values.

