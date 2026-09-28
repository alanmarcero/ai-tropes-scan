# AI Tropes Scan

A skill for AI coding agents that finds AI writing tropes in prose and rewrites them out. It checks word choice ("delve", "leverage", "quietly"), sentence patterns ("It's not X, it's Y", "The result? Devastating."), tone, formatting (em dashes, bold-first bullets) and document structure.

The catalog comes from [tropes.fyi](https://tropes.fyi) by [ossama.is](https://ossama.is). This repo condenses it into a skill file.

## Install

### Claude Code

```bash
mkdir -p ~/.claude/skills/ai-tropes-scan
cp SKILL.md ~/.claude/skills/ai-tropes-scan/SKILL.md
```

### Other AI agents

`SKILL.md` is plain markdown. Point your agent at it or paste it into a system prompt.

## Usage

```
/ai-tropes-scan
```

Paste the text you want checked. It also triggers on "tropes-check this", "scan for AI tells" or "make this sound less like AI".

To match your own voice, add a section of personal style rules to your CLAUDE.md or to your copy of `SKILL.md`.
