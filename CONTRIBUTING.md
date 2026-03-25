# Contributing to sharp-skills

Build this repository like a real marketplace, not a random pile of skill folders.

## What belongs here

A skill is a good fit when it is:
- reusable across multiple tasks or users
- clear about what it does and when it should trigger
- structured cleanly enough for long-term maintenance
- useful enough to justify cataloging and packaging

## Skill structure

Each skill should live under:

```text
skills/<skill-name>/
  SKILL.md
  references/    (optional)
  scripts/       (optional)
  assets/        (optional)
```

## Contribution checklist

Before publishing a skill:

1. Use a lowercase hyphenated name
2. Write clear YAML frontmatter with `name` and `description`
3. Keep `SKILL.md` concise
4. Move detailed guidance into `references/` when appropriate
5. Package the skill into `dist/`
6. Add or update the `skills-index.json` entry
7. Update docs if the public catalog changed

## Quality bar

Aim for:
- clear trigger conditions
- practical workflow guidance
- minimal fluff
- stable folder structure
- no duplicate or stale documentation

Avoid:
- vague descriptions
- giant monolithic `SKILL.md` files
- publishing unfinished placeholders
- committing secrets, tokens, or private data

## Versioning and maintenance

When updating a published skill:
- keep metadata accurate
- refresh the packaged artifact if the skill changed
- update indexes and docs together
- prefer incremental, reviewable commits

## Repository philosophy

This repository should feel curated. If a skill is not ready to be discovered, reused, and maintained, it is not ready to be published here.
