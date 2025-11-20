# Nocturne VS Code Theme

Minimal scaffold for the Nocturne theme.

## Structure

- `package.json` — VS Code extension manifest
- `themes/Nocturne-color-theme.json` — actual theme colors

## Building

1. Install Node.js (LTS).
2. Install vsce:

   ```bash
   npm install -g @vscode/vsce
   ```

3. From this folder:

   ```bash
   vsce package
   ```

4. Install the generated `.vsix` in VS Code.
