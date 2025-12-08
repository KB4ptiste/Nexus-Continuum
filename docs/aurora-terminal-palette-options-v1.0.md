# Aurora Nexus · Terminal Palette Options (v1.0)

This file defines **two full 16‑color terminal palettes** for the Aurora Nexus VS Code theme.

- **Option 1 – Functional / higher contrast**  
  Darker, more legible colors tuned for Aurora’s light background.
- **Option 2 – Softer / more pastel**  
  Closer to the Nocturne hues, but lower contrast. Better aesthetics, weaker accessibility.

Paste one option’s block into the `colors` section of `aurora-nexus.json`. Keep your existing `terminal.background` and `terminal.foreground` unless you deliberately want to change them.

Current defaults (for reference):

```jsonc
"terminal.background": "#E4D8FB",
"terminal.foreground": "#6D5B98",
"terminal.ansiCyan": "#33B9A6",
"terminal.ansiBrightCyan": "#52C7B8"
```

---

## Option 1 – Functional / higher contrast

This option uses darker, more muted hues for better readability on `#E4D8FB`.

```jsonc
// Aurora · Terminal (Option 1 – functional)
"terminal.selectionBackground": "#D7C6F733",

"terminal.ansiBlack":        "#6D5B98",
"terminal.ansiRed":          "#B2685A",
"terminal.ansiGreen":        "#4C8C46",
"terminal.ansiYellow":       "#96774C",
"terminal.ansiBlue":         "#8471BD",
"terminal.ansiMagenta":      "#BA5D8B",
"terminal.ansiCyan":         "#44877C",
"terminal.ansiWhite":        "#241B2F",

"terminal.ansiBrightBlack":  "#4A3C65",
"terminal.ansiBrightRed":    "#CC7B67",
"terminal.ansiBrightGreen":  "#3F9F55",
"terminal.ansiBrightYellow": "#A88450",
"terminal.ansiBrightBlue":   "#927BCA",
"terminal.ansiBrightMagenta":"#C46897",
"terminal.ansiBrightCyan":   "#3F9A88",
"terminal.ansiBrightWhite":  "#120A1F"
```

Notes:

- `ansiBlack` and `ansiBrightBlack` are tied to your muted text and plum neutrals.
- Reds / yellows map to error / warning semantics.
- White / bright white are very dark neutrals, which is typical for light‑background terminals where “white” often means “normal text color,” not literal white.

---

## Option 2 – Softer / pastel Aurora

This option stays closer to the original Nocturne hues but darkens them **just enough** to stay readable on `#E4D8FB`. Bright variants are lighter, more pastel.

```jsonc
// Aurora · Terminal (Option 2 – pastel)
"terminal.selectionBackground": "#D7C6F733",

"terminal.ansiBlack":        "#6D5B98",
"terminal.ansiRed":          "#E08371",
"terminal.ansiGreen":        "#5EAD57",
"terminal.ansiYellow":       "#BD955F",
"terminal.ansiBlue":         "#A68EED",
"terminal.ansiMagenta":      "#EB76B0",
"terminal.ansiCyan":         "#56AB9D",
"terminal.ansiWhite":        "#241B2F",

"terminal.ansiBrightBlack":  "#4A3C65",
"terminal.ansiBrightRed":    "#E69C8D",
"terminal.ansiBrightGreen":  "#7EBD79",
"terminal.ansiBrightYellow": "#CAAA7F",
"terminal.ansiBrightBlue":   "#B8A5F1",
"terminal.ansiBrightMagenta":"#EF91C0",
"terminal.ansiBrightCyan":   "#78BCB1",
"terminal.ansiBrightWhite":  "#120A1F"
```

Notes:

- Pastel variants are more “Aurora” in character but some bright colors have low contrast for heavy text usage.
- Use this if aesthetics matter more than strict readability for long terminal sessions.
