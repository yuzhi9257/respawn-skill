# 自研技能

自研 ZCode 技能仓库，本地 git 管理，后期上传 GitHub。

## 技能清单

| 技能 | 说明 |
|---|---|
| [respawn](respawn/SKILL.md) | 复活点：旧会话 token 耗尽/中断后，在新窗口断点续作任务，最小 token 消耗 |

## 使用方式

技能目录需位于 ZCode 发现路径下才能生效。本仓库通过软链接挂到用户级目录：

```bash
ln -s "$(pwd)/respawn" ~/.agents/skills/respawn
```

发现优先级（高→低）：`<项目>/.zcode/skills/` → `<项目>/.agents/skills/` → `~/.zcode/skills/` → `~/.agents/skills/`。
