# respawn-skill

[English](README_EN.md)

可复用的 AI 编码代理技能集。遵循开放的 [Agent Skills](https://agentskills.io) 规范，Claude Code / Codex / Cursor / ZCode 等 20 余种客户端通用，复制或软链即用。

## 技能列表

### [respawn](respawn/SKILL.md) 🎮

断点续作：旧会话因 token 耗尽或中断后，在新窗口从存档点复活任务，最小 token 消耗。

触发示例：

- "继续 sess_xxx"
- "上个窗口的任务没做完"
- "token 用完了帮我接着做"

## 安装

一条命令安装（[skills CLI](https://skills.sh/)）：

```bash
npx skills add yuzhi9257/respawn-skill
```

或手动软链到技能目录：

```bash
git clone https://github.com/yuzhi9257/respawn-skill.git
ln -s "$(pwd)/respawn-skill/respawn" ~/.agents/skills/respawn
```

## 目录结构

每个技能一个目录，`SKILL.md` 以 YAML frontmatter 声明 `name`/`description`，正文为 Markdown。

```
respawn/
└── SKILL.md
```

## 许可证

[MIT](LICENSE)
