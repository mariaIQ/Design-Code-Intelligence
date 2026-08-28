# Contributing

Contributions should improve a real design-to-production decision without turning a skill into a generic prompt collection.

## Before proposing a change

- Describe the user problem or repeated failure the change addresses.
- Keep instructions specific enough to alter useful behaviour, but narrow enough to avoid unrelated tasks.
- Preserve evidence, accessibility and authorisation boundaries.
- Avoid duplicated guidance that Codex already handles reliably.

## Skill changes

Each skill must include valid YAML frontmatter with a discriminating `name` and `description`. Keep the main `SKILL.md` concise; place substantial conditional detail in a focused reference only when needed.

Validate changed skills and the plugin before opening a pull request:

```bash
python3 /path/to/skill-creator/scripts/quick_validate.py skills/<skill-name>
python3 /path/to/plugin-creator/scripts/validate_plugin.py .
```

Explain the observable improvement and any trade-offs in the pull request description.
