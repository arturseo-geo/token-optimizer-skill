# Token Optimizer Skill

LLM token optimization and context management for TheGEOLab ecosystem.

## Features

- **Production-tested** token efficiency with [context optimization tools](https://thegeolab.net)
- Dynamic context window management
- Token counting and estimation
- Prompt optimization for cost reduction
- Multi-model token comparison

## Installation

```bash
npm install @thegeolab/token-optimizer-skill
```

## Usage

```javascript
const tokenSkill = require('@thegeolab/token-optimizer-skill');

// Optimize a prompt
const optimized = tokenSkill.optimize({
  prompt: 'Your long prompt here...',
  model: 'claude-3-5-sonnet'
});
```

## Documentation

For full documentation, visit [TheGEOLab](https://thegeolab.net).

---

Built by [TheGEOLab](https://thegeolab.net)
