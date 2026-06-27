# website-builder

## Custom Skills

Project-level slash commands live in `.claude/commands/`. Each `.md` file in that directory becomes a `/command-name` skill available across all Claude Code platforms (CLI, web, IDE extensions).

### Adding a new skill

1. Create `.claude/commands/<skill-name>.md`
2. Write the prompt/instructions that should run when the skill is invoked
3. Commit and push — the skill is immediately available on every platform

### Using arguments

Skills can reference `$ARGUMENTS` to capture whatever the user types after the command name:

```
/my-skill some text here
```

Inside the markdown file, `$ARGUMENTS` expands to `some text here`.

### Referencing files

Use `@filename` syntax inside a skill's markdown to pull file contents into the prompt at invocation time.

## Skills in this repo

| Command | File | Purpose |
|---------|------|---------|
| `/add-component` | `.claude/commands/add-component.md` | Scaffold a new UI component |

## Project overview

A website builder project. See individual skill files in `.claude/commands/` for available automations.
