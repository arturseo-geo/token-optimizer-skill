# Security Policy

## Scope

This skill is a set of Markdown instruction files for Claude Code. It does not
execute code directly, but it instructs Claude Code to modify settings and
environment variables that affect API costs and model behaviour. Security
matters.

## Supported Versions

| Version | Supported |
|---|---|
| Latest on `main` | Yes |
| Older commits | No |

## Reporting a Vulnerability

If you discover a security issue, **do not open a public issue**.

Instead, email **artur@thegeolab.net** with:
- Description of the vulnerability
- Steps to reproduce
- Potential impact
- Suggested fix (if you have one)

You will receive a response within 7 days. If the issue is confirmed, a fix
will be released and you will be credited (unless you prefer anonymity).

## Security Considerations for This Skill

### API key exposure
- This skill never references specific API keys or credentials
- Settings recommendations use environment variable names only
- Cost tracking advice directs users to Anthropic's dashboard, not to
  log credentials locally

### Settings manipulation
- The skill recommends changes to `.claude/settings.json` and environment
  variables
- All recommended settings are documented Anthropic features
- No recommendations involve undocumented or unsupported configuration

### Cost-related risks
- Incorrect pricing advice could cause unexpected API spend
- All cost figures should be verified against official Anthropic documentation
- The skill clearly labels estimates vs exact figures

### Model routing risks
- Routing complex security tasks to Haiku could miss vulnerabilities
- The skill explicitly recommends Opus for security audits
- Users should verify model choice is appropriate for security-sensitive work

## Best Practices for Users

1. **Verify pricing** against Anthropic's official pricing page before setting budgets
2. **Set API spend limits** in the Anthropic console as a safety net
3. **Do not commit settings.json** if it contains sensitive environment paths
4. **Review model routing** before security-sensitive tasks -- do not downgrade
   to save money on security audits
5. **Monitor API usage** through the official dashboard, not through local logs
   that could be tampered with
