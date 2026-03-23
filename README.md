# token-optimizer-skill

> Built by **[Artur Ferreira](https://github.com/arturseo-geo)** @ **[The GEO Lab](https://thegeolab.net)**
> [𝕏 @TheGEO_Lab](https://x.com/TheGEO_Lab) · [LinkedIn](https://linkedin.com/in/arturgeo) · [Reddit](https://www.reddit.com/user/Alternative_Teach_74/)

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![Licence](https://img.shields.io/badge/licence-MIT-green)
![Savings](https://img.shields.io/badge/typical_savings-60--80%25-orange)
![Claude Code](https://img.shields.io/badge/Claude_Code-skill-blueviolet)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)](https://github.com/arturseo-geo/token-optimizer-skill/blob/main/CONTRIBUTING.md)

Token cost optimisation skill for [Claude Code](https://docs.anthropic.com/en/docs/claude-code) — model routing, extended thinking tuning, prompt caching, subagent cost management, CLAUDE.md audit, MCP token audit, and per-session cost tracking. Typically reduces costs by 60-80%.

## Who This Is For

- **Anyone paying for Claude Code** who wants the same quality for less
- **Team leads** managing Claude Code costs across multiple developers
- **Power users** running long sessions who want to understand where tokens go
- **Agent builders** optimising multi-agent pipelines for cost efficiency

## What Makes This Different

Most cost advice is "use a cheaper model." This skill gives you a complete optimisation framework:

- ✅ **Model routing strategy** — Opus vs Sonnet vs Haiku decision framework with cost/quality tradeoffs
- ✅ **Extended thinking tuning** — when it helps vs. hurts, MAX_THINKING_TOKENS sweet spots
- ✅ **Prompt caching mechanics** — how cache hits work, how to optimise for them
- ✅ **Subagent cost management** — CLAUDE_CODE_SUBAGENT_MODEL routing for background agents
- ✅ **CLAUDE.md audit checklist** — find and fix token waste in your project instructions
- ✅ **MCP token audit** — tool descriptions that silently consume context
- ✅ **Per-session cost tracking** — know exactly what each session costs

## Quick Start

Add these three settings to `.claude/settings.json` for immediate savings:

```json
{
  "model": "sonnet",
  "env": {
    "MAX_THINKING_TOKENS": "10000",
    "CLAUDE_CODE_SUBAGENT_MODEL": "haiku"
  }
}
```

This alone typically reduces costs by 60-80% compared to Opus defaults.

## Install

```bash
# Clone
git clone https://github.com/arturseo-geo/token-optimizer-skill.git ~/.claude/skills/token-optimizer

# Or install all 12 skills at once
git clone https://github.com/arturseo-geo/claude-code-skills.git
cp -r claude-code-skills/skills/token-optimizer ~/.claude/skills/
```

## File Structure

```
token-optimizer-skill/
├── SKILL.md                  — Core skill: settings, routing, patterns, checklists
├── references/
│   ├── model-routing.md      — Opus vs Sonnet vs Haiku: cost, quality, decision framework
│   ├── thinking-tokens.md    — Extended thinking costs, tuning, when it helps vs hurts
│   ├── caching.md            — Prompt caching mechanics, cache hit optimisation
│   └── cost-tracking.md      — Per-session, per-task, per-project cost tracking
└── .github/                  — Issue templates and PR template
```

## Related Repos

- [claude-code-skills](https://github.com/arturseo-geo/claude-code-skills) — Full collection of 12 skills
- [context-engineering-skill](https://github.com/arturseo-geo/context-engineering-skill) — Companion skill for context window management

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines. PRs welcome.

---

Built and maintained by **[Artur Ferreira](https://github.com/arturseo-geo)** @ **[The GEO Lab](https://thegeolab.net)** · [MIT License](LICENSE)
