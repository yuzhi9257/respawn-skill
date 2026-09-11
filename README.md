# agent-skills

Reusable skills for AI coding agents — 可复用的 AI 编码代理技能集。遵循开放的 [Agent Skills](https://agentskills.io) 规范，Claude Code / Codex / Cursor / ZCode 等 20+ 客户端通用，复制或软链即用。

## Skills

### [respawn](respawn/SKILL.md) 🎮

断点续作：旧会话因 token 耗尽或中断"阵亡"后，在新窗口从存档点复活任务，最小 token 消耗。

**Use when:**
- "继续 sess_xxx"
- "上个窗口的任务没做完"
- "token 用完了帮我接着做"

## Install

一条命令安装（[skills CLI](https://skills.sh/)）：

```bash
npx skills add yuzhi9257/zcode-skills@respawn
```

或手动软链到任意客户端的技能目录：

```bash
git clone https://github.com/yuzhi9257/zcode-skills.git
ln -s "$(pwd)/zcode-skills/respawn" ~/.agents/skills/respawn
```

## Structure

每个技能一个目录：`SKILL.md`（YAML frontmatter 声明 `name`/`description` + Markdown 正文）。

```
respawn/
└── SKILL.md
```

## License

[MIT](LICENSE)
