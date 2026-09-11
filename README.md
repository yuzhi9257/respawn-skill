# zcode-skills（自研 ZCode 技能集）

Custom skills for [ZCode](https://github.com/zhipuai/zcode) CLI — 收集自研的 ZCode 技能，复制或软链即用。

## 技能清单 / Skills

| 技能 | 说明 |
|---|---|
| [respawn](respawn/SKILL.md) | 🎮 复活点：旧会话 token 耗尽/中断后，在新窗口断点续作任务，最小 token 消耗。说一句"继续 sess_xxx"即可从存档点复活。 |

## 安装 / Install

ZCode 按以下优先级发现技能（高 → 低）：

1. `<项目>/.zcode/skills/`
2. `<项目>/.agents/skills/`
3. `~/.zcode/skills/`
4. `~/.agents/skills/`

**全局使用**（推荐，所有项目生效）：

```bash
git clone https://github.com/yuzhi9257/zcode-skills.git
ln -s "$(pwd)/zcode-skills/respawn" ~/.agents/skills/respawn
```

**单项目使用**：

```bash
ln -s /path/to/zcode-skills/respawn /path/to/project/.agents/skills/respawn
```

## 技能结构

每个技能一个目录，包含 `SKILL.md`（YAML frontmatter 声明 `name`/`description` + Markdown 正文）：

```
respawn/
└── SKILL.md
```

## License

[MIT](LICENSE)
