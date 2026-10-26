# Character Skills

可复用的角色人格 Skill 集合。每个子目录都是一个独立的角色 Skill，包含 `SKILL.md` 与对应的调研、设定和辅助资料。

> 本项目为同人角色扮演 Skill，非官方授权作品。角色及相关作品版权归原作者与权利方所有。

## 技能列表

| 技能 | 角色 | 作品 | 说明 |
| --- | --- | --- | --- |
| [`meguru`](./meguru/) | 因幡巡（因幡めぐる / Inaba Meguru） | 《魔女的夜宴》（柚子社） | 基于官方中文版游戏原文与社区资料提炼的人格模型、行为启发式与表达 DNA |
| [`reverse1999-37`](./reverse1999-37/) | 37（Thirty-seven） | 《重返未来：1999》 | 基于官方主线、活动剧情、角色轶事与语音等资料蒸馏的角色扮演 Skill |

## 目录结构

```text
character-skills/
├─ README.md
├─ .gitattributes
├─ meguru/
│  ├─ SKILL.md
│  ├─ references/
│  └─ scripts/
└─ reverse1999-37/
   ├─ SKILL.md
   ├─ manifest.json
   ├─ README.md
   ├─ prompts/
   └─ references/
```

## 使用方法

1. 克隆本仓库：

   ```bash
   git clone https://github.com/<your-name>/character-skills.git
   ```

2. 将需要的技能目录复制到你的 agent skills 目录，例如：

   - OpenCode：`~/.config/opencode/skills/`
   - Claude Code：`~/.claude/skills/`

   Windows 下 `~` 通常对应 `%USERPROFILE%`。

3. 重启或重新加载 agent 后，通过角色名、作品名或 Skill 名称触发。

### 示例

- `用巡的视角分析一下这件事`
- `扮演37，给我讲讲质数`
- `Ciallo～`
- `37 会怎么理解这个证明？`

## 说明

- 各技能的具体触发条件、角色边界和扮演规则见对应目录下的 `SKILL.md`。
- `references/` 保存角色调研与设定资料，`scripts/` 保存资料处理脚本，可按需使用。
- 资料更新时间和覆盖范围记录在各自的 `manifest.json` 或 `SKILL.md` 中。
