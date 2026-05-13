# Hermes Skills Overview 中文公开索引

这是一个**脱敏后的公开版 Hermes Skills 功能索引**，用于快速查看：

- 当前有哪些 Skill 分类
- 每个 Skill 大致是做什么的
- 如何把某个 Skill 安装到自己的 Hermes 里
- 如何给这个索引仓库补充说明

## 文档入口

- [中文功能说明](./SKILLS_CN.md)
- [如何添加 Hermes Skill](./ADD_SKILL_GUIDE.md)

## 这个仓库和私有备份仓库的区别

- **公开仓库**：只放中文索引、分类说明、添加方法
- **私有仓库**：保存完整 `~/.hermes/skills` 备份压缩包和校验文件

## 如何使用这份索引

1. 先在 `SKILLS_CN.md` 里找到你感兴趣的分类或 Skill 名称
2. 如果你想把某个 Skill 装到自己的 Hermes：
   - 在 Hermes CLI 里运行 `hermes skills install <技能名或 URL>`
   - 或在会话中使用 `/skill <技能名>` 加载
3. 安装后可用 `hermes skills list` 查看已安装技能
4. 不确定时，先用 `hermes skills inspect <技能名>` 预览，再决定是否安装

## 如何给自己的 Hermes 添加 Skill

> 下面说的是把 Skill 加到你自己的 Hermes 环境，不是给这个公开仓库加压缩包。

### 方法一：安装已有 Skill

```bash
# 方式 1：按技能名安装
hermes skills install <skill-name>

# 方式 2：按 GitHub/直链 URL 安装
hermes skills install https://example.com/SKILL.md

# 查看是否安装成功
hermes skills list
```

### 方法二：自己编写 Skill

一个 Skill 通常至少包含：

- `SKILL.md`
- 前置说明（什么时候用）
- 功能说明（能做什么）
- 推荐命令或操作步骤
- 常见坑和验证方法

示例结构：

```text
my-skill/
└── SKILL.md
```

示例头部：

```md
---
name: my-skill
description: "Explain what this skill does"
---
```

### 方法三：给这个公开索引补充内容

如果你想修改这个仓库：

- 只补充中文说明
- 不要加入完整压缩包
- 不要加入 `.env`、key、token、私有路径
- 有新分类或新 Skill 时，再更新 `SKILLS_CN.md`

## 安全说明

本仓库**不包含**：

- 完整 skills 压缩包
- Release 备份附件
- 原始脚本
- `references/` 文件
- 私有配置、密钥、`.env`、token

完整备份保留在私有仓库中。
