# Platform Support

`sharp-skills` is maintained as a multi-platform skill marketplace repository.

## Target platforms

### Claude Code
Supported through:
- `.claude-plugin/plugin.json`
- `.claude-plugin/marketplace.json`

### Cursor
Supported through:
- `.cursor-plugin/plugin.json`

### Codex-like workflows
Supported through:
- `.codex/INSTALL.md`
- direct use of `skills/` and packaged artifacts in `dist/`

### OpenCode
Supported through:
- `.opencode/INSTALL.md`
- `.opencode/plugins/sharp-skills.js`
- `package.json`

### Gemini CLI
Supported through:
- `gemini-extension.json`
- `GEMINI.md`

## Support model

The repository aims to provide:
- discoverable skill source under `skills/`
- packaged distribution artifacts under `dist/`
- platform metadata for major code agents
- installation documentation that can grow with the catalog

## Current state

Platform support currently focuses on packaging, discovery, and installation compatibility. Deeper platform-native automation can be added incrementally as the marketplace grows.
