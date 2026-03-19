# skills

A collection of [Daemon Protocol](https://daemonprotocol.com) agent skills.

## Install a skill

```bash
npx skills add ares-system/skills --skill <skill-name>
```

Install all skills at once:

```bash
npx skills add ares-system/skills --all
```

## Available skills

| Skill | Description |
|---|---|
| [ares-system](./ares-system/) | AI-powered security platform with 8 tools: Trident (Solana fuzzing), Semgrep, FuzzyAI, HexStrike, Whistleblower, Checked Math, MCP Injection, Multi-Agent orchestration |
| [cyclops](./cyclops/) | Cryptocurrency wallet risk analysis — sanctions screening (OFAC), AML/KYC, blockchain graph analysis, entity labeling for ETH/SOL/BTC |
| [daemon-intelligence](./daemon-intelligence/) | Daemon-AI platform API — auth, chat completions, MCP tools, finance, blockchain intelligence |
| [obscura-privacy](./obscura-privacy/) | Post-quantum secure privacy vault — Arcium MPC confidential computing, ZK compression (Light Protocol), WOTS+ signatures, stealth addresses |

## Usage examples

```bash
# Install all skills
npx skills add ares-system/skills --all

# Install individual skills
npx skills add ares-system/skills --skill daemon-intelligence
npx skills add ares-system/skills --skill ares-system
npx skills add ares-system/skills --skill cyclops
npx skills add ares-system/skills --skill obscura-privacy
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
