# Nexus Continuum – VS Code Theme Pack

Nexus Continuum is a dual-mode theme collection for Visual Studio Code, designed around a shared orbital accent system. It contains:

- **Nocturne Nexus** — Deep, atmospheric dark mode built on violet-space tones.
- **Aurora Nexus** — Light, lavender-tinted counterpart using the same semantic structure.

Both themes use the same brand accent families, ensuring visual continuity across light and dark environments.

---

## Features

- Two fully matched themes inside one extension:
  - `Nocturne Nexus` (dark)
  - `Aurora Nexus` (light)
- Shared accent palette for consistent UI behavior
- Carefully tuned foreground/background contrast
- Stable semantic color mapping for token scopes
- Designed to work cleanly with:
  - VS Code UI chrome
  - Syntax highlighting
  - Git colors
  - Breadcrumbs, minimap, diff views, and diagnostics

---

## Screenshots

### Nocturne Nexus (Dark)
*(Insert screenshot)*

### Aurora Nexus (Light)
*(Insert screenshot)*

---

## Installation

### From VS Code Marketplace
(Once published)
1. Open **Extensions** panel (`Ctrl+Shift+X`).
2. Search for **Nexus Continuum**.
3. Install and select either theme.

### Manual Installation (Local VSIX)

```bash
vsce package
code --install-extension nexus-continuum-1.0.0.vsix
```

---

## Activating a Theme

Use the Command Palette:

```
CTRL / CMD + Shift + P → Preferences: Color Theme
```

Select:
- **Nocturne Nexus** for dark mode
- **Aurora Nexus** for light mode

---

## Auto-Switching Light & Dark Themes

Add to your `settings.json`:

```json
"window.autoDetectColorScheme": true,
"workbench.preferredDarkColorTheme": "Nocturne Nexus",
"workbench.preferredLightColorTheme": "Aurora Nexus"
```

---

## Folder Structure

```
Nexus-Continuum/
│ package.json
│ README.md
│ LICENSE
│
├─ media/
│   nexus-continuum-icon.png
│   nexus-continuum-banner.png
│   preview-nocturne.png
│   preview-aurora.png
│
└─ themes/
    nocturne-nexus.json
    aurora-nexus.json
```

---

## Theme Philosophy

### Core Goals
- Maintain legible contrast in all UI contexts
- Provide a cohesive visual identity across light/dark modes
- Reinforce continuum design through consistent accent use
- Keep syntax highlighting predictable and readable

### Accent Families
- **Purple** → brand identity
- **Magenta** → emphasis, keywords
- **Cyan / Teal** → motion, cursor, operational elements
- **Warm tones** → warnings, diffs, diagnostics

---

## Contributing

1. Fork the repository
2. Create a feature branch
3. Submit a pull request

Include screenshots when modifying color tokens.

---

## License

Released under the **MIT License**.