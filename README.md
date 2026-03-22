# token-optimizer-skill

> **Also available as part of [claude-code-skills](https://github.com/arturseo-geo/claude-code-skills)** -- a collection of 12 production-tested skills for Claude Code.

> Built by **[Artur Ferreira](https://github.com/arturseo-geo)** @ **[The GEO Lab](https://thegeolab.net)**
> [X @TheGEO_Lab](https://x.com/TheGEO_Lab) | [LinkedIn](https://linkedin.com/in/arturgeo) | [Reddit](https://www.reddit.com/user/Alternative_Teach_74/)

![Licence](https://img.shields.io/badge/licence-MIT-green)
![Claude Code](https://img.shields.io/badge/Claude_Code-skill-blueviolet)

Reduce Claude Code token consumption and API costs without sacrificing output quality. Covers model routing, extended thinking tuning, prompt caching, subagent cost management, and session-level cost tracking.

## Install

```bash
git clone https://github.com/arturseo-geo/token-optimizer-skill.git ~/.claude/skills/token-optimizer
```

## File Structure

```
token-optimizer-skill/
├── SKILL.md                  — Core skill: settings, routing, patterns, checklists
├── README.md                 — This file
├── CONTRIBUTING.md           — Contribution guidelines
├── SECURITY.md               — Security policy
├── LICENSE                   — MIT licence
├── .gitignore
├── references/
│   ├── model-routing.md      — Opus vs Sonnet vs Haiku: cost, quality, decision framework
│   ├── thinking-tokens.md    — Extended thinking costs, tuning, when it helps vs hurts
│   ├── caching.md            — Prompt caching mechanics, cache hit optimisation
│   └── cost-tracking.md      — Per-session, per-task, per-project cost tracking
└── .github/
    ├── ISSUE_TEMPLATE/
    │   ├── bug-report.md     — Bug report template
    │   └── platform-update.md — Pricing/model update template
    └── pull_request_template.md — PR template
```

## What This Skill Covers

| Topic | Location |
|---|---|
| Token cost breakdown | SKILL.md |
| Settings tuning (MAX_THINKING_TOKENS, subagent model, compaction) | SKILL.md |
| Model routing strategy | SKILL.md + references/model-routing.md |
| Prompt efficiency patterns | SKILL.md |
| Caching strategies | SKILL.md + references/caching.md |
| CLAUDE.md audit checklist | SKILL.md |
| MCP token audit | SKILL.md |
| Extended thinking tuning | SKILL.md + references/thinking-tokens.md |
| Batch request optimisation | SKILL.md |
| Cost-per-session analysis | SKILL.md + references/cost-tracking.md |

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

## Related Repos

- [claude-code-skills](https://github.com/arturseo-geo/claude-code-skills) -- Full collection of 12 skills
- [mcp-wordpress-setup](https://github.com/arturseo-geo/mcp-wordpress-setup) -- WordPress MCP server setup

## Acknowledgments

Built following the open-source best practice approach -- reading community work for inspiration, writing original content, and crediting every source.

**Based on:**
- [Agent Skills specification](https://github.com/anthropics/skills) by Anthropic (Apache 2.0)

All skill content is original writing. No files were copied or adapted from any source.

## Author

Built and maintained by **[Artur Ferreira](https://github.com/arturseo-geo)** @ **[The GEO Lab](https://thegeolab.net)**

## License

[MIT](LICENSE)
