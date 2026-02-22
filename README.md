# VS Code Terminal Grids

Instant terminal grid layouts for VS Code using `runCommands` keybindings. One keypress creates a full grid of terminal editors — no extensions needed.

## Keybindings

| Keybinding | Grid | Terminals |
|---|---|---|
| `Ctrl+Alt+Shift+4` | 2x2 | 4 |
| `Ctrl+Alt+Shift+6` | 3x2 | 6 |
| `Ctrl+Alt+Shift+9` | 3x3 | 9 |
| `Ctrl+Alt+Shift+3` | 4x3 | 12 |
| `Ctrl+Alt+Shift+1` | 4x4 | 16 |
| `Ctrl+Alt+Shift+0` | Close all | - |

Grid dimensions are listed as **columns x rows**.

## How It Works

Each keybinding uses VS Code's built-in `runCommands` to chain together terminal creation and split commands. For example, a 2x2 grid:

1. Closes all editors
2. Creates terminal editors side-by-side (columns)
3. Splits each column downward (rows)
4. Fills each split with a new terminal

The result is an evenly-spaced grid of independent terminal editors.

## Installation

1. Open VS Code
2. Open the Keyboard Shortcuts JSON file:
   - Press `Cmd+K` then `Cmd+S` to open Keyboard Shortcuts
   - Click the file icon in the top-right to open the JSON editor
   - Or use the Command Palette: **Preferences: Open Keyboard Shortcuts (JSON)**
3. Copy the contents of `keybindings.json` from this repo into your keybindings file
4. If you already have keybindings, merge the entries into your existing array

## Note for Mac Users

These keybindings use `Ctrl+Alt+Shift` as the modifier. Depending on your keyboard and VS Code configuration, you may need to swap `Ctrl` for `Cmd`. For example:

- `Ctrl+Alt+Shift+4` becomes `Cmd+Alt+Shift+4`

## License

MIT
