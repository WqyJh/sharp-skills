# sharp-skills

A general-purpose marketplace repository for reusable agent skills.

`sharp-skills` is designed to be a clean, extensible home for high-quality skills that can be installed, browsed, packaged, and maintained like a serious open source project.

The repository currently includes two presentation-oriented skills as its initial published entries, but the project itself is **not** limited to frontend presentation workflows.

## Goals

- Provide a curated home for reusable agent skills
- Keep skill source, packaged artifacts, and marketplace metadata in one place
- Make skills easy to discover, review, install, and extend
- Maintain a repository structure that can scale beyond a handful of skills

## Current published skills

### presentation-microsite
Build narrative microsites, scrollytelling pages, launch pages, annual report experiences, and interactive showcase websites.

### presentation-stage-app
Build linear stage-controlled presentation web apps for live talks, demos, keynotes, internal reviews, and polished deck-like experiences.

## Repository layout

```text
.claude-plugin/          Marketplace metadata
.codex/                  Codex-oriented installation notes
skills/                  Skill source folders
  <skill-name>/
dist/                    Packaged .skill artifacts
docs/                    Repository documentation and indexes
skills-index.json        Machine-readable published skill index
```

## Principles

- Keep `SKILL.md` concise and trigger-aware
- Put detailed guidance in `references/` when needed
- Prefer maintainable structure over one-off dumps
- Package published skills so they can be distributed cleanly
- Keep repository metadata in sync with actual published content

## Installation

### Generic workflow

1. Clone this repository.
2. Choose a skill from `skills/`.
3. Copy the skill folder into your agent platform's supported skills directory, or use the packaged artifact from `dist/` if your workflow expects `.skill` packages.
4. Start a new session and trigger the skill with an appropriate request.

### Codex-like workflows
See `.codex/INSTALL.md`.

## Publishing model

A published skill should usually include:
- a complete `SKILL.md`
- any required `references/`, `scripts/`, or `assets/`
- a packaged `.skill` artifact in `dist/`
- an entry in `skills-index.json`
- corresponding documentation updates when needed

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).

In short:
1. Add a new skill under `skills/<skill-name>`
2. Keep the skill focused and reusable
3. Package it into `dist/`
4. Update `skills-index.json`
5. Update docs if the published catalog changes

## Roadmap direction

The repository starts with presentation-focused skills, but is intended to grow into a broader marketplace covering categories such as:
- development workflows
- content and media
- research and analysis
- operations and automation
- design systems and communication

## License

MIT License. See [LICENSE](LICENSE).
