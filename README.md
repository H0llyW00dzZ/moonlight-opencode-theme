# 🌌 Moonlight theme for opencode.ai

A minimal, frameless dark theme for opencode.ai inspired by the [moonlight](https://github.com/atomiks/moonlight-vscode-theme) VS Code theme.

## Features

- Semantic color coding (errors in red, types darker, etc.)
- Minimal visual noise for better focus
- Optimized for truecolor terminals
- Based on the moonlight color palette

## Installation

### Global Installation

1. Create the themes directory:
```bash
mkdir -p ~/.config/opencode/themes
```

2. Download the theme file:
```bash
curl -o ~/.config/opencode/themes/moonlight.json https://raw.githubusercontent.com/h0llyw00dzz/moonlight-opencode-theme/master/.opencode/themes/moonlight.json
```

That's it! The theme is now available globally in opencode.ai.

## Usage

### Using the theme

1. Open opencode.ai
2. Type `/theme` and select `moonlight`
3. Or add it to your `opencode.json` config:

```json
{
  "$schema": "https://opencode.ai/config.json",
  "theme": "moonlight"
}
```

### Terminal Requirements

For best results, ensure your terminal supports **truecolor** (24-bit color):

- Check support: `echo $COLORTERM` (should output `truecolor` or `24bit`)
- Enable if needed: `export COLORTERM=truecolor`

Most modern terminals (iTerm2, Alacritty, Kitty, Windows Terminal, GNOME Terminal) support this by default.

## Color Palette

The theme uses the moonlight color scheme with comprehensive color definitions:

### Core Colors
- **Background**: `#222436` (dark blue-gray)
- **Focus/Panel**: `#1e2030` (medium gray-blue)
- **Primary**: `#82aaff` (light blue)
- **Accent**: `#86e1fc` (bright cyan)
- **Strong Teal**: `#4fd6be` (vibrant teal)

### Semantic Colors
- **Error**: `#ff757f` (hot red)
- **Warning**: `#ff966c` (bright orange)
- **Success**: `#c3e88d` (bright green)
- **Info**: `#65bcff` (bright sky blue)

### Text Colors
- **Primary Text**: `#c8d3f5` (light gray)
- **Muted Text**: `#828bb8` (darker gray)
- **Off White**: `#d5def8` (very light blue)

### Additional Colors
- **Pink**: `#fca7ea` (soft pink)
- **Desaturated Blue**: `#7a88cf` (muted blue)
- **Bluish Gray**: `#444a73` (blue-gray)
- **Selection**: `#717cb425` (transparent blue)

## Theme Structure

```
.opencode/themes/
└── moonlight.json    # Main theme file
```

The theme follows the opencode.ai JSON theme format with:
- Color definitions in the `defs` section
- Dark/light variants for all colors
- Semantic color mapping for UI elements and syntax highlighting

## License

MIT License - see [LICENSE](LICENSE) file for details.

## Acknowledgments

- Based on [moonlight](https://github.com/atomiks/moonlight-vscode-theme) by atomiks
- Originally inspired by various dark themes for better coding experience