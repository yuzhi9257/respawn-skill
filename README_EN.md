# respawn-skill

[中文](README.md)

Reusable skills for AI coding agents. Follows the open [Agent Skills](https://agentskills.io) spec and works with Claude Code, Codex, Cursor, ZCode, and 20+ other clients. Copy or symlink to use.

## Skills

### [respawn](respawn/SKILL.md) 🎮

Resume a task from its checkpoint after the previous session died from token exhaustion or interruption, with minimal token cost.

**Use when:**

- "continue sess_xxx"
- "the task in my last window isn't finished"
- "ran out of tokens, pick up where it left off"

## Install

One command via the [skills CLI](https://skills.sh/):

```bash
npx skills add yuzhi9257/respawn-skill
```

Or symlink manually into your agent's skills directory:

```bash
git clone https://github.com/yuzhi9257/respawn-skill.git
ln -s "$(pwd)/respawn-skill/respawn" ~/.agents/skills/respawn
```

## Structure

One directory per skill. `SKILL.md` declares `name`/`description` in YAML frontmatter, followed by a Markdown body.

```
respawn/
└── SKILL.md
```

## License

[MIT](LICENSE)
