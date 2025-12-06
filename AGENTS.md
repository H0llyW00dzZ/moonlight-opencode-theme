# AGENTS.md for moonlight-opencode-theme

## Build/Lint/Test Commands
- No build commands; themes are static JSON files.
- Lint: Validate JSON syntax with `jq . .opencode/themes/*.json` or `python -m json.tool .opencode/themes/*.json`.
- Test: Manually validate themes against opencode.ai schema at https://opencode.ai/theme.json. For single test: `jq . .opencode/themes/moonlight.json` to check syntax.

## Code Style Guidelines
- **Formatting**: 2-space indentation, double quotes for strings, trailing commas allowed.
- **Naming**: Color defs use lowercase camelCase (e.g., "gray1", "blue"). Theme keys use camelCase (e.g., "primary", "background").
- **Types**: All values are strings (hex colors or references). No types beyond JSON schema.
- **Imports**: None; themes are self-contained.
- **Error Handling**: Ensure themes validate against schema; avoid invalid hex or missing dark/light variants.
- **Structure**: Include "$schema", "defs" for colors, "theme" with dark/light objects referencing defs.
- **Consistency**: Match moonlight palette; use semantic colors for UI elements.
- **Editing**: Always read file first before editing to ensure changes apply correctly.
