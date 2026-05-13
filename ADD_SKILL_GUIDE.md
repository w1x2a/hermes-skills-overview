# 如何添加 Hermes Skill

这份文档面向想要把 Skill 加到自己 Hermes 环境、或者想给公开索引补充说明的人。

## 1. 安装别人已经写好的 Skill

### 1.1 从 Skill Hub / 已知名称安装

```bash
hermes skills install <skill-name>
hermes skills list
```

### 1.2 从 URL 安装

如果对方给你的是 `SKILL.md` 直链：

```bash
hermes skills install https://example.com/path/to/SKILL.md
hermes skills list
```

### 1.3 先预览再安装

```bash
hermes skills inspect <skill-name-or-url>
hermes skills install <skill-name-or-url>
```

## 2. 在会话中加载 Skill

安装后，在 Hermes 会话中可以显式加载：

```text
/skill <skill-name>
```

也可以启动时预加载：

```bash
hermes -s <skill-name>
hermes --skills <skill-name>
```

多个 Skill 可以逗号分隔或重复传参，具体以你本机 Hermes 版本为准。

## 3. 自己写一个 Skill

最小结构：

```text
my-skill/
└── SKILL.md
```

推荐结构：

```text
my-skill/
├── SKILL.md
├── references/
│   └── api-notes.md
├── scripts/
│   └── verify.sh
└── templates/
    └── example.md
```

`SKILL.md` 最小示例：

```md
---
name: my-skill
description: "一句话说明这个 Skill 什么时候用、能做什么。"
---

# My Skill

## 什么时候使用

当用户需要……时使用。

## 工作流程

1. 先检查……
2. 再执行……
3. 最后验证……

## 常见坑

- 不要把密钥写进文档。
- 不要假设用户环境一定有某个命令。

## 验证

```bash
your-command --version
```
```

## 4. 放到本地 Hermes skills 目录

通常安装后的 Skill 位于：

```bash
~/.hermes/skills/
```

如果是手写 Skill，可以放在类似路径：

```bash
mkdir -p ~/.hermes/skills/custom/my-skill
cp SKILL.md ~/.hermes/skills/custom/my-skill/SKILL.md
hermes skills list
```

如果你使用 Profile，多 Profile 的 skills 目录可能在对应 profile 下，请以本机 `hermes config path` 和 `hermes profile show <name>` 输出为准。

## 5. 给本公开索引补充内容

这个仓库是公开索引，不放原始完整 Skill 包。贡献时请遵守：

### 可以提交

- `README.md` 的说明优化
- `SKILLS_CN.md` 的分类、功能说明、安装指引
- `ADD_SKILL_GUIDE.md` 的流程补充
- 不含敏感信息的示例命令

### 不要提交

- 完整 `~/.hermes/skills` 压缩包
- `.env`、token、cookie、key、SSH 私钥
- `references/`、`scripts/`、`assets/` 原始目录
- 私有服务地址、内部账号、真实 API Key

## 6. 提交前自检

```bash
# 不应该出现压缩包或敏感文件
find . -type f \( -name '*.tar.gz' -o -name '*.zip' -o -name '.env*' -o -name '*.pem' -o -name '*.key' \) -print

# 简单敏感词扫描，仅作为辅助，不代表绝对安全
python3 - <<'PYSCAN'
from pathlib import Path
keywords = ['credential-like marker', 'private-key marker', 'environment file marker']
for path in Path('.').rglob('*'):
    if path.is_file():
        data = path.read_text(encoding='utf-8', errors='ignore').lower()
        if any(k in data for k in keywords):
            print(path)
PYSCAN
```

如果有命中，先确认是不是示例占位符；不确定就不要公开。
