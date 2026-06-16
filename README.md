# Hacker Terminal Theme

A dark, terminal-inspired color theme for VS Code, built around a deep near-black background (`#0d0f12`) with a muted green accent (`#2f9e6e`).

## Features

- **Editor** — dark background, muted green cursor and active line number, subtle selection highlight.
- **Sidebar / Activity Bar / Status Bar** — consistent dark surfaces with green accents for active/highlighted elements.
- **Terminal colors** — matches the editor palette so the integrated terminal feels native to the theme.
- **Bracket pair colorization** — nested brackets cycle through green, yellow, purple, and blue for easy matching.
- **Git decorations** — added/modified/deleted/untracked files are color-coded in the file explorer.
- **Syntax highlighting**
  - Control-flow keywords (`if`, `else`, `for`, `while`, `return`) — red, bold
  - Other keywords / storage types — green, bold
  - Constants / `const` declarations — light green, italic
  - Strings — yellow; template literals — brighter yellow; regex — red
  - Functions — purple
  - Decorators (`@Override`, Python decorators) — pink, italic
  - `this` / `self` — blue, italic
  - Comments — muted gray, italic

## Installation (local use)

1. Clone this repo.
2. Open the folder in VS Code.
3. Press `F5` to launch an Extension Development Host with the theme active, **or**
4. Package it permanently:
   ```bash
   npm install -g vsce
   vsce package
   ```
   Then install the generated `.vsix` file via Extensions panel → `...` menu → "Install from VSIX".

## Customization

All colors are defined in `themes/Terminal-Theme-color-theme.json`. The palette is built around two core colors:

| Purpose | Color |
|---|---|
| Background | `#0d0f12` |
| Accent (green) | `#2f9e6e` |
| Accent hover/bright | `#4ab98a` |

Change these two values and most of the theme's mood will shift accordingly.

## Why this exists

Built as a personal VS Code theme project — started from wanting a more "terminal-like" aesthetic to pair with Cascadia Code/JetBrains Mono, and extended over time with deeper syntax scoping and UI coverage (minimap, peek-view, git diff colors, etc.).