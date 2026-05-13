# Hermes Skills 中文功能说明

> 生成时间：2026-05-13T14:11:13  
> 来源目录：`~/.hermes/skills`  
> 当前统计：**126 个 Skills**，覆盖 **52 个分类**。

## 这是什么？

Hermes Skill 是一组可复用的任务能力包，通常包含：触发场景、标准操作流程、推荐命令、验证方法、常见坑位和相关参考文件。它的作用是让 Agent 在处理具体任务时不用从零摸索，而是调用已经沉淀好的工作流。

本仓库是当前环境中 `~/.hermes/skills` 的**公开中文索引**。你可以把它当成“目录 + 说明书”，先看懂有哪些能力，再决定要不要安装到自己的 Hermes。

完整压缩包仍保留在私有仓库中。

## 文档入口

- [如何添加 Hermes Skill](./ADD_SKILL_GUIDE.md)

## 如何使用这份索引

1. 先在下面的分类中找到你关心的 Skill。
2. 如果想把它加到自己的 Hermes 里：
   - 运行 `hermes skills install <技能名或 URL>`
   - 或在会话中输入 `/skill <技能名>`
3. 安装后用 `hermes skills list` 检查是否成功。
4. 不确定是否要装时，先用 `hermes skills inspect <技能名>` 预览。

## 如何给自己的 Hermes 添加 Skill

### 安装已有 Skill

```bash
hermes skills install <skill-name>
hermes skills install https://example.com/SKILL.md
hermes skills list
```

### 自己编写 Skill

一个 Skill 通常包含：

- `SKILL.md`
- 触发场景
- 功能说明
- 推荐命令或操作流程
- 常见坑和验证方法

### 给本仓库补充说明

- 只补充中文索引和说明
- 不要加入完整备份包
- 不要加入 `.env`、token、key 或私有路径
- 有新 Skill 时可更新对应分类条目

## 快速总览

- **Apple 生态** `apple`：5 个
- **自主 AI 代理** `autonomous-ai-agents`：4 个
- **创意生成** `creative`：19 个
- **数据科学** `data-science`：1 个
- **DevOps / 运维** `devops`：5 个
- **产品自测** `dogfood`：1 个
- **邮件** `email`：1 个
- **游戏服务器** `gaming`：2 个
- **GitHub 工作流** `github`：6 个
- **知识图谱** `graphify`：1 个
- **飞书审批** `lark-approval`：1 个
- **飞书考勤** `lark-attendance`：1 个
- **飞书多维表格** `lark-base`：1 个
- **飞书日历** `lark-calendar`：1 个
- **飞书通讯录** `lark-contact`：1 个
- **飞书文档** `lark-doc`：1 个
- **飞书云盘** `lark-drive`：1 个
- **飞书事件** `lark-event`：1 个
- **飞书即时消息** `lark-im`：1 个
- **飞书邮箱** `lark-mail`：1 个
- **飞书 Markdown** `lark-markdown`：1 个
- **飞书妙记** `lark-minutes`：1 个
- **飞书 OKR** `lark-okr`：1 个
- **飞书 OpenAPI 探索** `lark-openapi-explorer`：1 个
- **飞书共享基础** `lark-shared`：1 个
- **飞书电子表格** `lark-sheets`：1 个
- **飞书 Skill 制作** `lark-skill-maker`：1 个
- **飞书幻灯片** `lark-slides`：1 个
- **飞书任务** `lark-task`：1 个
- **飞书视频会议** `lark-vc`：1 个
- **飞书会议 Agent** `lark-vc-agent`：1 个
- **飞书画板** `lark-whiteboard`：1 个
- **飞书知识库** `lark-wiki`：1 个
- **飞书会议纪要工作流** `lark-workflow-meeting-summary`：1 个
- **飞书日程待办日报** `lark-workflow-standup-report`：1 个
- **MCP 集成** `mcp`：1 个
- **媒体处理** `media`：6 个
- **MLOps** `mlops`：1 个
- **模型评估** `mlops/evaluation`：2 个
- **模型推理部署** `mlops/inference`：4 个
- **模型/多模态** `mlops/models`：2 个
- **ML 研究** `mlops/research`：1 个
- **模型训练** `mlops/training`：3 个
- **笔记** `note-taking`：1 个
- **生产力工具** `productivity`：11 个
- **红队测试** `red-teaming`：1 个
- **研究检索** `research`：6 个
- **智能家居** `smart-home`：1 个
- **社交媒体** `social-media`：1 个
- **软件开发** `software-development`：12 个
- **网页访问** `web-access`：2 个
- **腾讯元宝** `yuanbao`：1 个

## 分类与功能明细

### Apple 生态 `apple`

- **apple-notes**：管理 Apple Notes via memo CLI: create, search, 编辑.  
  路径：`apple/apple-notes/SKILL.md`
- **apple-reminders**：Apple Reminders via remindctl: add, list, complete.（用于该领域的标准化自动化流程）  
  路径：`apple/apple-reminders/SKILL.md`
- **findmy**：Track Apple devices/AirTags via FindMy.app on macOS.（用于该领域的标准化自动化流程）  
  路径：`apple/findmy/SKILL.md`
- **imessage**：Send and receive iMessages/SMS via the imsg CLI on macOS.（用于该领域的标准化自动化流程）  
  路径：`apple/imessage/SKILL.md`
- **macos-computer-use**：该 Skill 提供对应场景的自动化操作流程、命令约束和常见坑位说明。  
  路径：`apple/macos-computer-use/SKILL.md`

### 自主 AI 代理 `autonomous-ai-agents`

- **claude-code**：委托编码任务给 to Claude Code CLI (features, PRs).  
  路径：`autonomous-ai-agents/claude-code/SKILL.md`
- **codex**：委托编码任务给 to OpenAI Codex CLI (features, PRs).  
  路径：`autonomous-ai-agents/codex/SKILL.md`
- **hermes-agent**：配置、扩展或贡献 Hermes Agent。  
  路径：`autonomous-ai-agents/hermes-agent/SKILL.md`
- **opencode**：委托编码任务给 to OpenCode CLI (features, PR review).  
  路径：`autonomous-ai-agents/opencode/SKILL.md`

### 创意生成 `creative`

- **architecture-diagram**：生成深色风格 SVG 架构/云/基础设施图。  
  路径：`creative/architecture-diagram/SKILL.md`
- **ascii-art**：生成 ASCII 艺术: pyfiglet, cowsay, boxes, image-to-ascii.  
  路径：`creative/ascii-art/SKILL.md`
- **ascii-video**：ASCII video: convert video/audio to colored ASCII MP4/GIF.（用于该领域的标准化自动化流程）  
  路径：`creative/ascii-video/SKILL.md`
- **baoyu-comic**：Knowledge comics (知识漫画): educational, biography, tutorial.  
  路径：`creative/baoyu-comic/SKILL.md`
- **baoyu-infographic**：制作信息图: 21 layouts x 21 styles (信息图, 可视化).  
  路径：`creative/baoyu-infographic/SKILL.md`
- **claude-design**：设计 one-off HTML artifacts (landing, deck, prototype).  
  路径：`creative/claude-design/SKILL.md`
- **comfyui**：生成图片、视频和音频 with ComfyUI — install, launch, 管理 nodes/models, run workflows with parameter injection. Uses the official comfy-cli for lifecycle and direct REST/WebSocket API for execution.  
  路径：`creative/comfyui/SKILL.md`
- **design-md**：Author/validate/export Google's DESIGN.md token spec files.（用于该领域的标准化自动化流程）  
  路径：`creative/design-md/SKILL.md`
- **excalidraw**：Hand-drawn Excalidraw JSON diagrams (arch, flow, seq).（用于该领域的标准化自动化流程）  
  路径：`creative/excalidraw/SKILL.md`
- **humanizer**：Humanize text: strip AI-isms and add real voice.（用于该领域的标准化自动化流程）  
  路径：`creative/humanizer/SKILL.md`
- **ideation**：Generate project ideas via creative constraints.（用于该领域的标准化自动化流程）  
  路径：`creative/creative-ideation/SKILL.md`
- **manim-video**：Manim CE animations: 3Blue1Brown math/algo videos.（用于该领域的标准化自动化流程）  
  路径：`creative/manim-video/SKILL.md`
- **p5js**：p5.js sketches: gen art, shaders, interactive, 3D.（用于该领域的标准化自动化流程）  
  路径：`creative/p5js/SKILL.md`
- **pixel-art**：Pixel art w/ era palettes (NES, Game Boy, PICO-8).（用于该领域的标准化自动化流程）  
  路径：`creative/pixel-art/SKILL.md`
- **popular-web-designs**：54 real design systems (Stripe, Linear, Vercel) as HTML/CSS.（用于该领域的标准化自动化流程）  
  路径：`creative/popular-web-designs/SKILL.md`
- **pretext**：Use when building creative browser demos with @chenglou/pretext — DOM-free text layout for 生成 ASCII 艺术, typographic flow around obstacles, text-as-geometry games, kinetic typography, and text-powered generative art. Produces single-file HTML demos by default.  
  路径：`creative/pretext/SKILL.md`
- **sketch**：Throwaway HTML mockups: 2-3 design variants to compare.（用于该领域的标准化自动化流程）  
  路径：`creative/sketch/SKILL.md`
- **songwriting-and-ai-music**：Songwriting craft and Suno AI music prompts.（用于该领域的标准化自动化流程）  
  路径：`creative/songwriting-and-ai-music/SKILL.md`
- **touchdesigner-mcp**：Control a running Touch设计er instance via twozero MCP — create operators, set parameters, wire connections, execute Python, build real-time visuals. 36 native tools.  
  路径：`creative/touchdesigner-mcp/SKILL.md`

### 数据科学 `data-science`

- **jupyter-live-kernel**：Iterative Python via live Jupyter kernel (hamelnb).（用于该领域的标准化自动化流程）  
  路径：`data-science/jupyter-live-kernel/SKILL.md`

### DevOps / 运维 `devops`

- **kanban-orchestrator**：Decomposition playbook + specialist-roster conventions + anti-temptation rules for an orchestrator profile routing work through Kanban. The "don't do the work yourself" rule and the basic lifecycle are auto-injected into every kanban worker's system prompt; this skill is the deeper playbook when you're specifically playing the orchestrator role.（用于该领域的标准化自动化流程）  
  路径：`devops/kanban-orchestrator/SKILL.md`
- **kanban-worker**：Pitfalls, examples, and edge cases for Hermes Kanban workers. The lifecycle itself is auto-injected into every worker's system prompt as KANBAN_GUIDANCE (from agent/prompt_builder.py); this skill is what you load when you want deeper detail on specific scenarios.（用于该领域的标准化自动化流程）  
  路径：`devops/kanban-worker/SKILL.md`
- **remote-server-backup**：Use for backing up local state directories such as ~/.hermes to a remote VPS. Covers interactive SSH setup, enabling pubkey auth when disabled, avoiding broken tar archives, rsync with exclusions, and post-copy verification.（用于该领域的标准化自动化流程）  
  路径：`devops/remote-server-backup/SKILL.md`
- **webhook-subscriptions**：Webhook subscriptions: event-driven agent runs.（用于该领域的标准化自动化流程）  
  路径：`devops/webhook-subscriptions/SKILL.md`
- **wsl-windows-interop**：Use when operating from WSL against Windows resources: WSLg GUI apps, Docker Desktop containers, Windows-native project scaffolding, cmd/reg/browser interop, path translation, and no-sudo fallbacks.（用于该领域的标准化自动化流程）  
  路径：`devops/wsl-windows-interop/SKILL.md`

### 产品自测 `dogfood`

- **dogfood**：Exploratory QA of web apps: find bugs, evidence, reports.（用于该领域的标准化自动化流程）  
  路径：`dogfood/SKILL.md`

### 邮件 `email`

- **himalaya**：Himalaya CLI: IMAP/SMTP email from terminal.（用于该领域的标准化自动化流程）  
  路径：`email/himalaya/SKILL.md`

### 游戏服务器 `gaming`

- **minecraft-modpack-server**：Host modded Minecraft servers (CurseForge, Modrinth).（用于该领域的标准化自动化流程）  
  路径：`gaming/minecraft-modpack-server/SKILL.md`
- **pokemon-player**：Play Pokemon via headless emulator + RAM reads.（用于该领域的标准化自动化流程）  
  路径：`gaming/pokemon-player/SKILL.md`

### GitHub 工作流 `github`

- **codebase-inspection**：Inspect codebases w/ pygount: LOC, languages, ratios.（用于该领域的标准化自动化流程）  
  路径：`github/codebase-inspection/SKILL.md`
- **github-auth**：GitHub 认证配置: HTTPS tokens, SSH keys, gh CLI login.  
  路径：`github/github-auth/SKILL.md`
- **github-code-review**：审查 PR: diffs, inline comments via gh or REST.  
  路径：`github/github-code-review/SKILL.md`
- **github-issues**：创建, triage, label, assign GitHub issues via gh or REST.  
  路径：`github/github-issues/SKILL.md`
- **github-pr-workflow**：GitHub PR lifecycle: branch, commit, open, CI, merge.（用于该领域的标准化自动化流程）  
  路径：`github/github-pr-workflow/SKILL.md`
- **github-repo-management**：Clone/create/fork repos; 管理 remotes, releases.  
  路径：`github/github-repo-management/SKILL.md`

### 知识图谱 `graphify`

- **graphify**：any input (code, docs, papers, images) → knowledge graph → clustered communities → HTML + JSON + audit report（用于该领域的标准化自动化流程）  
  路径：`graphify/SKILL.md`

### 飞书审批 `lark-approval`

- **lark-approval**：飞书审批 API：审批实例、审批任务管理。  
  路径：`lark-approval/SKILL.md`

### 飞书考勤 `lark-attendance`

- **lark-attendance**：飞书考勤打卡：查询自己的考勤打卡记录  
  路径：`lark-attendance/SKILL.md`

### 飞书多维表格 `lark-base`

- **lark-base**：当需要用 lark-cli 操作飞书多维表格（Base）时调用：搜索 Base、建表、字段管理、记录读写、记录分享链接、视图配置、历史查询，以及角色/表单/仪表盘管理/工作流；也适用于把旧的 +table / +field / +record 写法改成当前命令写法。涉及字段设计、公式字段、查找引用、跨表计算、行级派生指标、数据分析需求时也必须使用本 skill。  
  路径：`lark-base/SKILL.md`

### 飞书日历 `lark-calendar`

- **lark-calendar**：飞书日历（calendar）：提供日历与日程（会议）的全面管理能力。核心场景包括：查看/搜索日程、创建/更新日程、管理参会人、查询忙闲状态及推荐空闲时段、查询/搜索与预定会议室。注意：涉及【预约日程/会议】或【查询/预定会议室】时，必须先读取 references/lark-calendar-schedule-meeting.md 工作流！高频操作请优先使用 Shortcuts：+agenda（快速概览今日/近期行程）、+create（创建日程并按需邀请参会人及预定会议室）、+update（更新既有日程字段，或独立增删参会人/会议室）、+freebusy（查询用户主日历的忙闲信息和rsvp的状态）、+rsvp（回复日程邀请）  
  路径：`lark-calendar/SKILL.md`

### 飞书通讯录 `lark-contact`

- **lark-contact**：飞书 / 飞书/Lark 通讯录,用于按姓名 / 邮箱把员工解析成 open_id,以及按 open_id 反查员工的姓名 / 部门 / 邮箱 / 联系方式。当用户说出某人姓名而下一步需要发消息 / 加群 / 排日程时,先用本 skill 把姓名换成 ID;当输出里出现 open_id 需要展示成姓名给用户看,或用户直接询问某人的部门 / 邮箱 / 联系方式时,用本 skill 查。不负责部门树遍历、按部门列员工、组织架构图,这类需求走原生 OpenAPI。  
  路径：`lark-contact/SKILL.md`

### 飞书文档 `lark-doc`

- **lark-doc**：飞书云文档（v2）：创建和编辑飞书文档。使用本 skill 时，docs +create、docs +fetch、docs +update 必须携带 --api-version v2；默认使用 DocxXML 格式（也支持 Markdown）。创建文档、获取文档内容（支持 simple/with-ids/full 三种导出详细度，以及 full/outline/range/keyword/section 五种局部读取模式，可按目录、block id 区间、关键词或标题自动成节只拉部分内容以节省上下文）、更新文档（八种指令：str_replace/block_insert_after/block_copy_insert_after/block_replace/block_delete/block_move_after/overwrite/append）、上传和下载文档中的图片和文件、搜索云空间文档。当用户需要创建或编辑飞书文档、读取文档内容、在文档中插入图片、搜索云空间文档时使用；如果用户是想按名称或关键词先定位电子表格、报表等云空间对象，也优先使用本 skill 的 docs +search 做资源发现。  
  路径：`lark-doc/SKILL.md`

### 飞书云盘 `lark-drive`

- **lark-drive**：飞书云空间：管理云空间中的文件和文件夹。上传和下载文件、创建文件夹、复制/移动/删除文件、查看文件元数据、管理文档评论、管理文档权限、订阅用户评论变更事件、修改文件标题（docx、sheet、bitable、file、folder、wiki）；也负责把本地 Word/Markdown/Excel/CSV 以及 Base 快照（.base）导入为飞书在线云文档（docx、sheet、bitable）。当用户需要上传或下载文件、整理云空间目录、查看文件详情、管理评论、管理文档权限、修改文件标题、订阅用户评论变更事件，或要把本地文件导入成新版文档、电子表格、多维表格/Base 时使用。  
  路径：`lark-drive/SKILL.md`

### 飞书事件 `lark-event`

- **lark-event**：飞书/Lark/Feishu real-time event listening / subscribing / consuming: stream events as NDJSON via `lark-cli event consume <EventKey>` (covers IM message receive, reactions, chat member changes, etc.). Use for 飞书/Lark bots, real-time message processing, long-running subscribers, streaming webhook/push handlers. Supports `--max-events` / `--timeout` bounded runs and a stderr ready-marker contract — designed for AI agents running as subprocesses.  
  路径：`lark-event/SKILL.md`

### 飞书即时消息 `lark-im`

- **lark-im**：飞书即时通讯：收发消息和管理群聊。发送和回复消息、搜索聊天记录、管理群聊成员、上传下载图片和文件（支持大文件分片下载）、管理表情回复。当用户需要发消息、查看或搜索聊天记录、下载聊天中的文件、查看群成员、管理标记数据时使用。  
  路径：`lark-im/SKILL.md`

### 飞书邮箱 `lark-mail`

- **lark-mail**：飞书邮箱 — draft, compose, send, reply, forward, read, and search emails; 管理 drafts, folders, labels, contacts, attachments, and mail rules. Use when user mentions 起草邮件, 写一封邮件, 拟邮件, 草稿, 发通知邮件, 发送邮件, 发邮件, 回复邮件, 转发邮件, 查看邮件, 看邮件, 读邮件, 搜索邮件, 查邮件, 收件箱, 邮件会话, 编辑草稿, 管理草稿, 下载附件, 邮件文件夹, 邮件标签, 邮件联系人, 监听新邮件, 收信规则, 邮件规则, draft, compose, send email, reply, forward, inbox, mail thread, mail rules.  
  路径：`lark-mail/SKILL.md`

### 飞书 Markdown `lark-markdown`

- **lark-markdown**：飞书 Markdown：查看、创建、上传和编辑 Markdown 文件。当用户需要创建或编辑 Markdown 文件、读取或修改时使用。  
  路径：`lark-markdown/SKILL.md`

### 飞书妙记 `lark-minutes`

- **lark-minutes**：飞书妙记：妙记相关基本功能。1.查询妙记列表（按关键词/所有者/参与者/时间范围）；2.获取妙记基础信息（标题、封面、时长 等）；3.下载妙记音视频文件；4.获取妙记相关 AI 产物（总结、待办、章节）；5.上传音视频生成妙记，也支持将本地音视频文件转成纪要、逐字稿、文字稿、撰写文字等产物。遇到这类请求时，应优先使用本 skill，而不是尝试 `ffmpeg`、`whisper` 等本地转写命令。飞书妙记 URL 格式: http(s)://<host>/minutes/<minute-token>  
  路径：`lark-minutes/SKILL.md`

### 飞书 OKR `lark-okr`

- **lark-okr**：飞书 OKR：管理目标与关键结果。查看和编辑 OKR 周期、目标（Objective）、关键结果（Key Result）、对齐关系、量化指标和进展记录。当用户需要查看或创建 OKR、管理目标和关键结果、查看对齐关系时使用。  
  路径：`lark-okr/SKILL.md`

### 飞书 OpenAPI 探索 `lark-openapi-explorer`

- **lark-openapi-explorer**：飞书/飞书/Lark 原生 OpenAPI 探索：从官方文档库中挖掘未经 CLI 封装的原生 OpenAPI 接口。当用户的需求无法被现有 lark-* skill 或 lark-cli 已注册命令满足，需要查找并调用原生飞书 OpenAPI 时使用。  
  路径：`lark-openapi-explorer/SKILL.md`

### 飞书共享基础 `lark-shared`

- **lark-shared**：飞书/飞书/Lark CLI 共享基础：应用配置初始化、认证登录（auth login）、身份切换（--as user/bot）、权限与 scope 管理、Permission denied 错误处理、安全规则。当用户需要第一次配置(`lark-cli config init`)、使用登录授权(`lark-cli auth login`)、遇到权限不足、切换 user/bot 身份、配置 scope、或首次使用 lark-cli 时触发。  
  路径：`lark-shared/SKILL.md`

### 飞书电子表格 `lark-sheets`

- **lark-sheets**：飞书电子表格：创建和操作电子表格。支持创建表格、创建/复制/删除/更新工作表、读写单元格、追加行数据、查找内容、导出文件。当用户需要创建电子表格、管理工作表、批量读写数据、在已知表格中查找内容、导出或下载表格时使用。若用户是想按名称或关键词搜索云空间里的表格文件，请改用 lark-doc 的 docs +search 先定位资源。  
  路径：`lark-sheets/SKILL.md`

### 飞书 Skill 制作 `lark-skill-maker`

- **lark-skill-maker**：创建 lark-cli 的自定义 Skill。当用户需要把飞书 API 操作封装成可复用的 Skill（包装原子 API 或编排多步流程）时使用。  
  路径：`lark-skill-maker/SKILL.md`

### 飞书幻灯片 `lark-slides`

- **lark-slides**：飞书幻灯片：创建和编辑幻灯片，接口通过 XML 协议通信。创建演示文稿、读取幻灯片内容、管理幻灯片页面（创建、删除、读取、局部替换）。当用户需要创建或编辑幻灯片、读取或修改单个页面时使用。  
  路径：`lark-slides/SKILL.md`

### 飞书任务 `lark-task`

- **lark-task**：飞书任务：管理任务、清单和任务智能体。创建待办任务、查看和更新任务状态、拆分子任务、组织任务清单、分配协作成员、上传任务附件、注册或注销任务智能体、更新任务智能体的主页数据、写入智能体任务记录。当用户需要创建待办事项、查看任务列表、跟踪任务进度、管理项目清单或给他人分配任务、为任务上传附件文件、注册注销任务智能体、更新智能体主页数据、写入任务记录时使用。  
  路径：`lark-task/SKILL.md`

### 飞书视频会议 `lark-vc`

- **lark-vc**：飞书视频会议：搜索历史会议、查询会议纪要产物（总结、待办、章节、逐字稿）、查询会议参会人快照。1. 查询已经结束的会议数量或详情时使用本技能（如历史日期｜昨天｜上周｜今天已经开过的会议等场景），查询未开始的会议日程使用 lark-calendar 技能。2. 支持通过关键词、时间范围、组织者、参与者、会议室等筛选条件搜索会议。3. 获取或整理会议纪要、逐字稿、录制产物时使用本技能。4. 查询“谁参加过某会议”“参会人列表”等参会人快照信息用 vc meeting get --with-participants（任意时点可查，含已结束会议）。注意：**Agent 真实入会/离会、感知正在进行中会议的实时事件**请使用 lark-vc-agent 技能，本技能不覆盖写操作和会中事件流。  
  路径：`lark-vc/SKILL.md`

### 飞书会议 Agent `lark-vc-agent`

- **lark-vc-agent**：飞书视频会议：让机器人代当前用户加入/离开正在进行的会议，并读取会议期间的实时事件（参会人加入与离开、发言、聊天、屏幕共享等）。1. 用户提供 9 位会议号、要求代为入会或离会时使用 +meeting-join / +meeting-leave——会真实产生入会/离会记录。2. 会议进行中用户想知道“谁加入了”“谁离开了”“谁在发言”“有人共享屏幕吗”等会中动态时，机器人入会后用 +meeting-events 读取事件时间线。3. 典型场景：参会机器人、会中助手、代为旁听、代为参会。前提：机器人只能读到它自己参会过且仍在进行中的会议的事件；查询已结束会议的参会名单、纪要或逐字稿请使用 lark-vc 技能。  
  路径：`lark-vc-agent/SKILL.md`

### 飞书画板 `lark-whiteboard`

- **lark-whiteboard**：>  
  路径：`lark-whiteboard/SKILL.md`

### 飞书知识库 `lark-wiki`

- **lark-wiki**：飞书知识库：管理知识空间、空间成员和文档节点。创建和查询知识空间、查看和管理空间成员、管理节点层级结构、在知识库中组织文档和快捷方式。当用户需要在知识库中查找或创建文档、浏览知识空间结构、查看或管理空间成员、移动或复制节点时使用。  
  路径：`lark-wiki/SKILL.md`

### 飞书会议纪要工作流 `lark-workflow-meeting-summary`

- **lark-workflow-meeting-summary**：会议纪要整理工作流：汇总指定时间范围内的会议纪要并生成结构化报告。当用户需要整理会议纪要、生成会议周报、回顾一段时间内的会议内容时使用。  
  路径：`lark-workflow-meeting-summary/SKILL.md`

### 飞书日程待办日报 `lark-workflow-standup-report`

- **lark-workflow-standup-report**：日程待办摘要：编排 calendar +agenda 和 task +get-my-tasks，生成指定日期的日程与未完成任务摘要。适用于了解今天/明天/本周的安排。  
  路径：`lark-workflow-standup-report/SKILL.md`

### MCP 集成 `mcp`

- **native-mcp**：MCP client: connect servers, register tools (stdio/HTTP).（用于该领域的标准化自动化流程）  
  路径：`mcp/native-mcp/SKILL.md`

### 媒体处理 `media`

- **feishu-voice-bubble-tts**：Use when sending TTS/audio replies in Feishu/飞书/Lark as native voice bubbles instead of MP3/file attachments. Covers ffmpeg/libopus setup, real Ogg Opus verification, MEDIA tag routing, and Hermes TTS edge cases.  
  路径：`media/feishu-voice-bubble-tts/SKILL.md`
- **gif-search**：搜索/download GIFs from Tenor via curl + jq.  
  路径：`media/gif-search/SKILL.md`
- **heartmula**：HeartMuLa: Suno-like song generation from lyrics + tags.（用于该领域的标准化自动化流程）  
  路径：`media/heartmula/SKILL.md`
- **songsee**：Audio spectrograms/features (mel, chroma, MFCC) via CLI.（用于该领域的标准化自动化流程）  
  路径：`media/songsee/SKILL.md`
- **spotify**：Spotify: play, search, queue, 管理 playlists and devices.  
  路径：`media/spotify/SKILL.md`
- **youtube-content**：YouTube 字幕 to summaries, threads, blogs.  
  路径：`media/youtube-content/SKILL.md`

### MLOps `mlops`

- **huggingface-hub**：HuggingFace hf CLI: search/download/upload models, datasets.（用于该领域的标准化自动化流程）  
  路径：`mlops/huggingface-hub/SKILL.md`

### 模型评估 `mlops/evaluation`

- **evaluating-llms-harness**：lm-eval-harness: 基准评测 LLMs (MMLU, GSM8K, etc.).  
  路径：`mlops/evaluation/lm-evaluation-harness/SKILL.md`
- **weights-and-biases**：W&B: log ML experiments, sweeps, model registry, dashboards.（用于该领域的标准化自动化流程）  
  路径：`mlops/evaluation/weights-and-biases/SKILL.md`

### 模型推理部署 `mlops/inference`

- **llama-cpp**：llama.cpp local GGUF inference + HF Hub model discovery.（用于该领域的标准化自动化流程）  
  路径：`mlops/inference/llama-cpp/SKILL.md`
- **obliteratus**：OBLITERATUS: abliterate LLM refusals (diff-in-means).（用于该领域的标准化自动化流程）  
  路径：`mlops/inference/obliteratus/SKILL.md`
- **outlines**：Outlines: structured JSON/regex/Pydantic LLM generation.（用于该领域的标准化自动化流程）  
  路径：`mlops/inference/outlines/SKILL.md`
- **serving-llms-vllm**：vLLM: high-throughput LLM serving, OpenAI API, quantization.（用于该领域的标准化自动化流程）  
  路径：`mlops/inference/vllm/SKILL.md`

### 模型/多模态 `mlops/models`

- **audiocraft-audio-generation**：AudioCraft: MusicGen text-to-music, AudioGen text-to-sound.（用于该领域的标准化自动化流程）  
  路径：`mlops/models/audiocraft/SKILL.md`
- **segment-anything-model**：SAM: zero-shot image segmentation via points, boxes, masks.（用于该领域的标准化自动化流程）  
  路径：`mlops/models/segment-anything/SKILL.md`

### ML 研究 `mlops/research`

- **dspy**：DSPy: declarative LM programs, auto-optimize prompts, RAG.（用于该领域的标准化自动化流程）  
  路径：`mlops/research/dspy/SKILL.md`

### 模型训练 `mlops/training`

- **axolotl**：Axolotl: YAML LLM 微调 (LoRA, DPO, GRPO).  
  路径：`mlops/training/axolotl/SKILL.md`
- **fine-tuning-with-trl**：TRL: SFT, DPO, PPO, GRPO, reward modeling for LLM RLHF.（用于该领域的标准化自动化流程）  
  路径：`mlops/training/trl-fine-tuning/SKILL.md`
- **unsloth**：Unsloth: 2-5x faster LoRA/QLoRA 微调, less VRAM.  
  路径：`mlops/training/unsloth/SKILL.md`

### 笔记 `note-taking`

- **obsidian**：读取, search, create, and 编辑 notes in the Obsidian vault.  
  路径：`note-taking/obsidian/SKILL.md`

### 生产力工具 `productivity`

- **airtable**：Airtable REST API via curl. Records CRUD, filters, upserts.（用于该领域的标准化自动化流程）  
  路径：`productivity/airtable/SKILL.md`
- **cad-quantity-takeoff**：Extract materials, dimensions, and budget-grade quantities from DWG/DXF/CAD drawings in WSL, with safe fallbacks for conversion, rendering, and visual verification.（用于该领域的标准化自动化流程）  
  路径：`productivity/cad-quantity-takeoff/SKILL.md`
- **google-workspace**：Gmail, Calendar, Drive, Docs, Sheets via gws CLI or Python.（用于该领域的标准化自动化流程）  
  路径：`productivity/google-workspace/SKILL.md`
- **linear**：Linear: 管理 issues, projects, teams via GraphQL + curl.  
  路径：`productivity/linear/SKILL.md`
- **maps**：Geocode, POIs, routes, timezones via OpenStreetMap/OSRM.（用于该领域的标准化自动化流程）  
  路径：`productivity/maps/SKILL.md`
- **nano-pdf**：Edit PDF text/typos/titles via nano-pdf CLI (NL prompts).（用于该领域的标准化自动化流程）  
  路径：`productivity/nano-pdf/SKILL.md`
- **notion**：Notion API via curl: pages, databases, blocks, search.（用于该领域的标准化自动化流程）  
  路径：`productivity/notion/SKILL.md`
- **ocr-and-documents**：Extract and validate text/tables from PDFs, scans, DOCX, and related documents using low-token local processing, OCR fallbacks, authoritative-source discipline, and targeted visual/table verification.（用于该领域的标准化自动化流程）  
  路径：`productivity/ocr-and-documents/SKILL.md`
- **powerpoint**：创建, read, 编辑 .pptx decks, slides, notes, templates.  
  路径：`productivity/powerpoint/SKILL.md`
- **ppt-beautify**：Use when beautifying, redesigning, polishing, or visually QA'ing existing PowerPoint decks, especially Chinese business/report decks. Turns rough PPTs into coherent, modern, presentation-ready decks with verified visuals.（用于该领域的标准化自动化流程）  
  路径：`productivity/ppt-beautify/SKILL.md`
- **teams-meeting-pipeline**：Operate the Teams meeting summary pipeline via Hermes CLI — summarize meetings, inspect pipeline status, replay jobs, 管理 Microsoft Graph subscriptions.  
  路径：`productivity/teams-meeting-pipeline/SKILL.md`

### 红队测试 `red-teaming`

- **godmode**：Jailbreak LLMs: Parseltongue, GODMODE, ULTRAPLINIAN.（用于该领域的标准化自动化流程）  
  路径：`red-teaming/godmode/SKILL.md`

### 研究检索 `research`

- **arxiv**：搜索 arXiv papers by keyword, author, category, or ID.  
  路径：`research/arxiv/SKILL.md`
- **blogwatcher**：Monitor blogs and RSS/Atom feeds via blogwatcher-cli tool.（用于该领域的标准化自动化流程）  
  路径：`research/blogwatcher/SKILL.md`
- **find-skills**：Helps users discover and install agent skills when they ask questions like "how do I do X", "find a skill for X", "is there a skill that can...", or express interest in extending capabilities. This skill should be used when the user is looking for functionality that might exist as an installable skill.（用于该领域的标准化自动化流程）  
  路径：`research/find-skills/SKILL.md`
- **llm-wiki**：Karpathy's LLM Wiki: build/query interlinked markdown KB.（用于该领域的标准化自动化流程）  
  路径：`research/llm-wiki/SKILL.md`
- **polymarket**：Query Polymarket: markets, prices, orderbooks, history.（用于该领域的标准化自动化流程）  
  路径：`research/polymarket/SKILL.md`
- **research-paper-writing**：Write ML papers for NeurIPS/ICML/ICLR: design→submit.（用于该领域的标准化自动化流程）  
  路径：`research/research-paper-writing/SKILL.md`

### 智能家居 `smart-home`

- **openhue**：Control Philips Hue lights, scenes, rooms via OpenHue CLI.（用于该领域的标准化自动化流程）  
  路径：`smart-home/openhue/SKILL.md`

### 社交媒体 `social-media`

- **xurl**：X/Twitter via xurl CLI: post, search, DM, media, v2 API.（用于该领域的标准化自动化流程）  
  路径：`social-media/xurl/SKILL.md`

### 软件开发 `software-development`

- **chrome-extension-cdp**：Chrome 扩展直连 CDP 控制，替代传统 CDP Proxy 模式，提升浏览器自动化效率 1000 倍。  
  路径：`software-development/chrome-extension-cdp/SKILL.md`
- **debugging-hermes-tui-commands**：Debug Hermes TUI slash commands: Python, gateway, Ink UI.（用于该领域的标准化自动化流程）  
  路径：`software-development/debugging-hermes-tui-commands/SKILL.md`
- **hermes-agent-skill-authoring**：Author in-repo SKILL.md: frontmatter, validator, structure.（用于该领域的标准化自动化流程）  
  路径：`software-development/hermes-agent-skill-authoring/SKILL.md`
- **node-inspect-debugger**：Debug Node.js via --inspect + Chrome DevTools Protocol CLI.（用于该领域的标准化自动化流程）  
  路径：`software-development/node-inspect-debugger/SKILL.md`
- **plan**：Plan mode: write markdown plan to .hermes/plans/, no exec.（用于该领域的标准化自动化流程）  
  路径：`software-development/plan/SKILL.md`
- **python-debugpy**：Debug Python: pdb REPL + debugpy remote (DAP).（用于该领域的标准化自动化流程）  
  路径：`software-development/python-debugpy/SKILL.md`
- **requesting-code-review**：Pre-commit review: security scan, quality gates, auto-fix.（用于该领域的标准化自动化流程）  
  路径：`software-development/requesting-code-review/SKILL.md`
- **spike**：Throwaway experiments to validate an idea before build.（用于该领域的标准化自动化流程）  
  路径：`software-development/spike/SKILL.md`
- **subagent-driven-development**：Execute plans via delegate_task subagents (2-stage review).（用于该领域的标准化自动化流程）  
  路径：`software-development/subagent-driven-development/SKILL.md`
- **systematic-debugging**：4-phase root cause debugging: understand bugs before fixing.（用于该领域的标准化自动化流程）  
  路径：`software-development/systematic-debugging/SKILL.md`
- **test-driven-development**：TDD: enforce RED-GREEN-REFACTOR, tests before code.（用于该领域的标准化自动化流程）  
  路径：`software-development/test-driven-development/SKILL.md`
- **writing-plans**：Write implementation plans: bite-sized tasks, paths, code.（用于该领域的标准化自动化流程）  
  路径：`software-development/writing-plans/SKILL.md`

### 网页访问 `web-access`

- **cloakbrowser-web-automation**：Use when browser automation needs CloakBrowser stealth Chromium, anti-detection Playwright automation, or a local CloakBrowser setup for web tasks.（用于该领域的标准化自动化流程）  
  路径：`web-access/cloakbrowser-web-automation/SKILL.md`
- **web-access**：所有联网操作必须通过此 skill 处理，包括：搜索、网页抓取、登录后操作、网络交互等。  
  路径：`web-access/SKILL.md`

### 腾讯元宝 `yuanbao`

- **yuanbao**：Yuanbao (元宝) groups: @mention users, query info/members.  
  路径：`yuanbao/SKILL.md`

## 公开版说明

这是一个**脱敏公开索引**，只展示 Hermes Skills 的分类和功能概览。

本公开仓库**不包含**：

- 完整 `~/.hermes/skills` 压缩包
- 任何 Release 备份附件
- 原始 `references/` 文件
- 脚本源码
- 本地配置、凭据或密钥
- 私有环境路径、token、cookie、`.env` 等敏感信息

如需恢复完整 skills，请使用私有备份仓库中的 Release 压缩包。
