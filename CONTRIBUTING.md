# Contributing to token-optimizer-skill

Thank you for your interest in improving this skill. This document explains
how to contribute effectively.

## Before You Start

1. **Check existing issues** -- your idea may already be tracked
2. **Read SKILL.md** -- understand the current optimisation strategies
3. **Read the references/** -- ensure your contribution does not duplicate existing content

## What You Can Contribute

### Pricing and model updates
- Updated token pricing when Anthropic changes rates
- New model additions (benchmarks, routing recommendations)
- Corrected cost estimates based on real-world measurements

### New optimisation strategies
- Techniques for reducing token consumption
- Workflow patterns that lower cost without sacrificing quality
- Tool-specific optimisations (MCP servers, subagent patterns)

### Cost data and benchmarks
- Real-world cost measurements for different task types
- Before/after comparisons when applying specific settings
- Team-scale cost analysis patterns

### Documentation
- Clearer explanations of existing strategies
- Examples and case studies
- Troubleshooting guides for common cost issues

## How to Submit Changes

1. **Fork the repository**
2. **Create a feature branch** from `main`:
   ```bash
   git checkout -b feature/your-change-name
   ```
3. **Make your changes** following the conventions below
4. **Test your changes** by applying the advice in a real Claude Code session
5. **Open a pull request** using the PR template

## Conventions

### File format
- All skill files are Markdown (`.md`)
- Use ATX-style headings (`#`, `##`, `###`)
- Use fenced code blocks with language identifiers
- Tables use pipe syntax with alignment
- Keep lines under 100 characters where practical

### Cost figures
- Always state which model the cost applies to
- Include the date or note "as of [month] [year]" for pricing
- Link to official Anthropic documentation when possible
- Use conservative estimates (round up costs, round down savings)

### Commit messages
- Use imperative mood: "Update Sonnet pricing" not "Updated Sonnet pricing"
- First line under 72 characters
- Explain why, not just what, in the body if the change is non-obvious

### Naming
- Reference files: `references/[topic].md` (lowercase, hyphenated)

## What We Will Not Merge

- Advice that encourages prompt injection or jailbreaking
- Cost figures without a verifiable source
- Changes that recommend disabling safety features
- Files that contain API credentials, tokens, or secrets
- Purely cosmetic changes with no functional benefit
- Advice specific to a single project (keep it general)

## Questions?

Open an issue with the question label, or start a discussion in the repository.

## License

By contributing, you agree that your contributions will be licensed under
the same MIT License that covers this project.
