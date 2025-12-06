# 🌌 Moonlight themes for [opencode.ai](https://github.com/sst/opencode)

Minimal, frameless dark themes for [opencode.ai](https://github.com/sst/opencode) inspired by the [moonlight](https://github.com/atomiks/moonlight-vscode-theme) VS Code theme.

## Available Themes

- **[Moonlight](.opencode/themes/moonlight.json)**: Classic dark theme with solid backgrounds
- **[Moonlight II](.opencode/themes/moonlight-ii.json)**: Alternative variant with refined color accents
- **[Moonlight III](.opencode/themes/moonlight-iii.json)**: Green-accented variant with yellow code elements, evoking lunar landscapes
- **[Moonlight Eclipse](.opencode/themes/moonlight-eclipse.json)**: Darker variant with crimson accents, evoking a blood moon lunar eclipse

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

2. Download the theme files:

#### Moonlight
```bash
curl -o ~/.config/opencode/themes/moonlight.json https://raw.githubusercontent.com/h0llyw00dzz/moonlight-opencode-theme/master/.opencode/themes/moonlight.json
```

#### Moonlight II
```bash
curl -o ~/.config/opencode/themes/moonlight-ii.json https://raw.githubusercontent.com/h0llyw00dzz/moonlight-opencode-theme/master/.opencode/themes/moonlight-ii.json
```

#### Moonlight III
```bash
curl -o ~/.config/opencode/themes/moonlight-iii.json https://raw.githubusercontent.com/h0llyw00dzz/moonlight-opencode-theme/master/.opencode/themes/moonlight-iii.json
```

#### Moonlight Eclipse
```bash
curl -o ~/.config/opencode/themes/moonlight-eclipse.json https://raw.githubusercontent.com/h0llyw00dzz/moonlight-opencode-theme/master/.opencode/themes/moonlight-eclipse.json
```

That's it! The themes are now available globally in [opencode.ai](https://github.com/sst/opencode).

## Usage

### Using the themes

1. Open [opencode.ai](https://github.com/sst/opencode)
  2. Type `/theme` and select `moonlight`, `moonlight-ii`, `moonlight-iii`, or `moonlight-eclipse`
3. Or add it to your `opencode.json` config:

```json
{
  "$schema": "https://opencode.ai/config.json",
  "theme": "moonlight"
}
```

or

```json
{
  "$schema": "https://opencode.ai/config.json",
  "theme": "moonlight-ii"
}
```

or

```json
{
  "$schema": "https://opencode.ai/config.json",
  "theme": "moonlight-iii"
}
```

or

```json
{
  "$schema": "https://opencode.ai/config.json",
  "theme": "moonlight-eclipse"
}
```

### Terminal Requirements

For best results, ensure your terminal supports **truecolor** (24-bit color):

- Check support: `echo $COLORTERM` (should output `truecolor` or `24bit`)
- Enable if needed: `export COLORTERM=truecolor`

Most modern terminals (iTerm2, Alacritty, Kitty, Windows Terminal, GNOME Terminal) support this by default.

## Color Palette

All themes use a corrected moonlight color scheme (~4100K temperature, neutral grays, toned blues) with comprehensive color definitions:

### Core Colors
- **Background**: `#101010` (dark neutral gray)
- **Panel**: `#202020` (muted neutral gray)
- **Primary**: `#6495ed` (cornflower blue)
- **Accent**: Varies by theme (blue in Moonlight, teal in II, green in III, red in Eclipse)

### Semantic Colors
- **Error**: `#dc143c` (crimson)
- **Warning**: `#daa520` (goldenrod)
- **Success**: `#228b22` (forest green) / `#2e8b57` (sea green in Eclipse)
- **Info**: `#6495ed` (cornflower blue)

### Text Colors
- **Primary Text**: `#f0f0f0` (light neutral gray)
- **Muted Text**: `#e0e0e0` (muted light gray)

### Additional Colors
- **Blues**: `#6495ed` (cornflower), `#4169e1` (royal blue)
- **Reds**: `#dc143c` (crimson), `#b22222` (firebrick)
- **Greens**: `#228b22` (forest), `#2e8b57` (sea green)
- **Yellow**: `#daa520` (goldenrod)

## Theme Structure

```
.opencode/themes/
├── moonlight.json         # Classic theme with solid backgrounds
├── moonlight-ii.json      # Enhanced theme with solid backgrounds
├── moonlight-iii.json     # Green-accented variant with yellow elements
└── moonlight-eclipse.json # Darker variant with red accents
```

The themes follow the [opencode.ai](https://github.com/sst/opencode) JSON theme format with:
- Color definitions in the `defs` section
- Dark/light variants for all colors
- Semantic color mapping for UI elements and syntax highlighting

## License

MIT License - see [LICENSE](LICENSE) file for details.

## Acknowledgments

- Based on [moonlight](https://github.com/atomiks/moonlight-vscode-theme) by atomiks
- Originally inspired by various dark themes for better coding experience
