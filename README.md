# 🌌 Moonlight themes for [opencode.ai](https://github.com/sst/opencode)

Minimal, frameless dark themes for [opencode.ai](https://github.com/sst/opencode) inspired by the [moonlight](https://github.com/atomiks/moonlight-vscode-theme) VS Code theme.

## Available Themes

- **[Moonlight](.opencode/themes/moonlight.json)**: Classic dark theme with blue-tinted grays and vibrant blues/teals
- **[Moonlight II](.opencode/themes/moonlight-ii.json)**: Alternative variant with blue-tinted grays and refined teal accents
- **[Moonlight III](.opencode/themes/moonlight-iii.json)**: Green-accented variant with neutral grays, toned blues, and yellow code elements, evoking lunar landscapes
- **[Moonlight Eclipse](.opencode/themes/moonlight-eclipse.json)**: Darker variant with deep red-tinted grays, blood moon reds (crimson, copper, mahogany), and amber glow for lunar eclipse effect

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

## Color Palettes

Themes use variations of the moonlight palette with comprehensive color definitions. Below are the key colors for each theme:

### Moonlight & Moonlight II
- **Grays**: Blue-tinted (#131421 to #d5def8)
- **Blues**: #82aaff (bright), #3d59a1 (dark), #65bcff (sky)
- **Teals**: #4fd6be, #7af8ca (light)
- **Greens**: #c3e88d
- **Yellows**: #ffc777
- **Reds**: #ff757f, #ff5370 (dark)
- **Accent**: Vibrant blues/teals

### Moonlight III
- **Grays**: Neutral (#101010 to #f0f0f0)
- **Blues**: #6495ed (toned), #4169e1 (dark), #87ceeb (sky)
- **Teals**: #20b2aa, #48d1cc (light)
- **Greens**: #c3e88d
- **Yellows**: #ffc777
- **Reds**: #ff757f, #ff5370 (dark)
- **Accent**: Green with yellow code elements

### Moonlight Eclipse
- **Grays**: Deep red-tinted (#0d0808 to #f5e6e6)
- **Blues**: #5f8dd3 (muted), #4169e1 (dark)
- **Reds**: #cc0000 (bloodRed), #dc143c (crimson), #8b0000 (darkCrimson), #b22222 (firebrick), #8b4513 (eclipseRust), #b87333 (eclipseCopper), #c04000 (eclipseMahogany)
- **Yellows/Oranges**: #daa520 (goldenrod), #ff8c00 (orange), #d4691a (eclipseAmber), #ffd700 (moonGlow)
- **Greens**: #2e8b57 (sea green)
- **Accent**: Blood moon reds with copper/amber highlights

### Semantic Colors
- **Error**: #ff757f (in Moonlight/II/III), #cc0000 (bloodRed in Eclipse)
- **Warning**: #ffc777 (in Moonlight/II/III), #d4691a (eclipseAmber in Eclipse)
- **Success**: #c3e88d (in Moonlight/II/III), #2e8b57 (sea green in Eclipse)
- **Info**: #82aaff (in Moonlight/II), #6495ed (in III/Eclipse)

## Theme Structure

```
.opencode/themes/
├── moonlight.json         # Classic theme with blue-tinted grays
├── moonlight-ii.json      # Enhanced theme with blue-tinted grays
├── moonlight-iii.json     # Green-accented variant with neutral grays
└── moonlight-eclipse.json # Darker variant with deep red-tinted grays
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
