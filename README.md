# Product Analyst Skill

A Claude Code skill that performs systematic product and business opportunity analysis from a brutal VC perspective.

> **[中文版本](SKILL.zh-CN.md)** | **[English Version](SKILL.md)**

## What It Does

When you describe a product idea, startup concept, or business partnership opportunity, this skill triggers a structured 9-module analysis:

1. **One-Line Verdict** — No hedging, no filler
2. **Target Audience** — Real users, real pain, decision chain
3. **Why Now** — Timing drivers: tech, market, regulation, competition
4. **Business Model** — Revenue logic, pricing, break-even math
5. **Competitive Landscape** — Who's alive, who's dead, and why
6. **Team & Execution Risk** — Founder-market fit, capability gaps
7. **MVP Definition** — Minimum cost validation with go/kill signals
8. **Scorecard** — 7 dimensions, 1-5 scale with reasoning
9. **Final Recommendation** — Go all in, validate first, or kill it

## Install

### Option 1: User-level (available in all projects)

```bash
mkdir -p ~/.claude/skills/product-analyst
# English
cp SKILL.md ~/.claude/skills/product-analyst/SKILL.md
# or Chinese
cp SKILL.zh-CN.md ~/.claude/skills/product-analyst/SKILL.md
```

### Option 2: Project-level (available in one project)

```bash
mkdir -p .claude/skills/product-analyst
# English
cp SKILL.md .claude/skills/product-analyst/SKILL.md
# or Chinese
cp SKILL.zh-CN.md .claude/skills/product-analyst/SKILL.md
```

## Usage

In Claude Code, just describe your product idea or business opportunity:

```
> Analyze my product: a note-taking app for medical students that uses AI to convert handwritten notes into structured study guides

> 帮我分析一下这个想法：做一个面向宠物主的SaaS平台，连接宠物医院和宠物主

> Is this partnership worth pursuing? Company X wants us to integrate their payment SDK...
```

Claude Code will automatically invoke the skill and run the full 9-module analysis.

## Design Principles

- **No hedging** — Forces clear yes/no/validate verdicts instead of vague "has potential"
- **Numbers over narratives** — Break-even calculations, market sizing, specific competitor data
- **Anti-confirmation bias** — Explicitly forbids manufacturing positives for balance
- **Information-aware** — Asks for missing context before analyzing, flags gaps that affect judgment
- **Kill signals** — Every MVP section includes explicit criteria for when to stop

## Requirements

- [Claude Code](https://docs.anthropic.com/en/docs/claude-code) CLI or IDE extension

## License

MIT
