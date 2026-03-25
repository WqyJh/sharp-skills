# Installing sharp-skills for OpenCode

## Installation

Add `sharp-skills` to the `plugin` array in your `opencode.json`:

```json
{
  "plugin": ["sharp-skills@git+https://github.com/WqyJh/sharp-skills.git"]
}
```

Restart OpenCode after updating the config.

## What this provides

- Access to the published skills shipped in this repository
- A reusable skills catalog that can grow over time

## Notes

- `sharp-skills` is a general-purpose skill marketplace repository.
- The current published catalog starts with presentation-oriented skills, but the repository is intended to support many categories.
- If your OpenCode setup expects direct skill paths instead of plugin-based loading, copy the desired skill folder from `skills/` manually.
