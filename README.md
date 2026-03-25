# sharp-skills

A curated skills marketplace repository for frontend presentation experiences that go beyond PPT.

This repository is inspired by the structure and distribution style of [obra/superpowers](https://github.com/obra/superpowers), but focuses on reusable presentation-building skills.

## Included skills

### 1. presentation-microsite
Build narrative microsites, scrollytelling pages, launch pages, annual report experiences, and interactive showcase websites.

Best for:
- scrollytelling
- narrative microsites
- campaign pages
- investor or strategy stories
- presentation websites meant to be shared after the meeting

### 2. presentation-stage-app
Build linear stage-controlled presentation web apps for live talks, demos, keynotes, internal reviews, and polished deck-like experiences.

Best for:
- keynote-style presentations
- live demos
- keyboard-controlled web decks
- presenter mode
- replacing PowerPoint with a component-based frontend presentation app

## Repository layout

```text
.claude-plugin/          Marketplace metadata
.codex/                  Codex installation notes
skills/                  Skill source folders
  presentation-microsite/
  presentation-stage-app/
dist/                    Packaged .skill artifacts
docs/                    Extra repository documentation
```

## Install / use

### OpenClaw
Copy a skill source folder into your workspace skills directory, or use the packaged `.skill` artifact if your workflow expects packaged skills.

### Codex / general agent workflows
Read the relevant `SKILL.md` and install/copy the skill into your agent's supported skills directory.

## Current focus

This marketplace starts with two presentation-focused skills, but is designed to grow into a broader library around:
- presentation systems
- storytelling UX
- motion systems
- demo sites
- media-rich frontend communication

## Contributing

1. Add a new skill under `skills/<skill-name>`
2. Keep `SKILL.md` concise and trigger-aware
3. Put detailed guidance in `references/`
4. Package the skill into `dist/` when ready
5. Update metadata files if you add a new published skill

## License

MIT License. See `LICENSE`.
