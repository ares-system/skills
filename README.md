# skills

A collection of [OpenCode](https://opencode.ai) agent skills.

## Install a skill

```bash
npx skills add fikriaf/skills --skill <skill-name>
```

Install all skills at once:

```bash
npx skills add fikriaf/skills --all
```

## Available skills

| Skill | Description |
|---|---|
| [daemon-intelligence](./daemon-intelligence/) | Complete reference for the Daemon-AI platform API — auth, chat completions, MCP tools, finance, blockchain intelligence |

## Usage example

```bash
# Install daemon-intelligence globally
npx skills add fikriaf/skills --skill daemon-intelligence -g

# Install into current project only
npx skills add fikriaf/skills --skill daemon-intelligence
```

## Adding a new skill

Each skill is a folder with a `SKILL.md` inside:

```
skills/
└── your-skill-name/
    ├── SKILL.md          ← required, must have name + description frontmatter
    └── references/       ← optional reference files loaded on demand
```

## License

MIT
