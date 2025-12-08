# Nocturne Nexus · Core UI & Git Decoration Options (v1.0)

This file provides **two option sets** for adding missing but useful UI colors to the Nocturne Nexus theme:

- `foreground`
- `focusBorder`
- `gitDecoration.*`
- `panelTitle.*`

Each option is a self‑contained snippet to add to the `colors` section of `nocturne-nexus.json`.

Current related keys (for reference):

```jsonc
"editor.foreground":           "#D8C5EE",
"titleBar.activeForeground":   "#D8C5EE",
"titleBar.inactiveForeground": "#977DB5",
"editorError.foreground":      "#FF9580",
"editorWarning.foreground":    "#FFCA80",
"editorInfo.foreground":       "#80FFEA"
```

---

## Option A – High‑clarity, aligned with existing semantics

Use this if you want Git decorations and panel titles to feel very explicit and readable.

```jsonc
// Nocturne · Core UI additions (Option A)
"foreground": "#D8C5EE",        // match editor.foreground

"focusBorder": "#80FFEA80",     // aqua focus ring (same family as find / cursor)

"panelTitle.activeForeground":   "#D8C5EE",
"panelTitle.inactiveForeground": "#977DB5",

// Git decoration colors (strong, semantic)
"gitDecoration.addedResourceForeground":       "#8AFF80",  // success green
"gitDecoration.modifiedResourceForeground":    "#FFCA80",  // warm amber
"gitDecoration.deletedResourceForeground":     "#FF9580",  // error red
"gitDecoration.untrackedResourceForeground":   "#A8FF9A",  // bright green
"gitDecoration.ignoredResourceForeground":     "#3E2E50",  // low‑contrast neutral
"gitDecoration.conflictingResourceForeground": "#FFB3A0",  // strong red/orange
"gitDecoration.submoduleResourceForeground":   "#80FFEA"   // aqua accent
```

Characteristics:

- Very clear state signaling in the Explorer.
- Focus ring uses the same aqua logic as your find highlights and cursor.

---

## Option B – Slightly softer / lavender‑biased

Use this if you want Git/status to be a little less loud but still readable.

```jsonc
// Nocturne · Core UI additions (Option B)
"foreground": "#B4A3C8",        // slightly softer than pure editor.foreground

"focusBorder": "#B399FF80",     // lavender focus ring

"panelTitle.activeForeground":   "#F5ECFF",  // lighter title for contrast
"panelTitle.inactiveForeground": "#B394D6",  // softer inactive title

// Git decoration colors (muted, still semantic)
"gitDecoration.addedResourceForeground":       "#8AFF80",  // keep readable green
"gitDecoration.modifiedResourceForeground":    "#FFCA80",
"gitDecoration.deletedResourceForeground":     "#FF9580",
"gitDecoration.untrackedResourceForeground":   "#C2FFB3",  // softer than A8FF9A
"gitDecoration.ignoredResourceForeground":     "#3E2E50",
"gitDecoration.conflictingResourceForeground": "#FFB3A0",
"gitDecoration.submoduleResourceForeground":   "#B399FF"   // use lavender instead of aqua
```

Characteristics:

- Panel titles stand out more from the dark chrome.
- Focus ring leans into the core lavender accent instead of aqua.
- Git decorations are still legible but less saturated in the “noisy” states (untracked, submodules).
