# RaiseAI Media Skills

> RaiseAI 媒体生成工具集 — 支持 Claude Code、OpenClaw、Codex、Cursor 等 AI 代理。

## 目录结构

```
raise-ai-skills/
└── skills/
    └── raise-ai-media/              # Agent Skills 标准版本
        ├── SKILL.md                 # 核心技能定义
        └── references/              # 参考文档
            ├── api-setup.md         # API Key 配置
            ├── image-generation.md   # 图片生成
            ├── video-generation.md   # 视频生成
            ├── script-generation.md # 脚本生成
            ├── prompt-extraction.md # 提示词反推
            └── polling-and-errors.md # 轮询与错误处理
```

## 安装方式

### Claude Code / Codex / Cursor / Cline 等

使用 [skills CLI](https://www.npmjs.com/package/skills)：

```bash
npx skills add Micrease-AI/raise-ai-skills --skill raise-ai-media
```

### OpenClaw

使用 [ClawHub CLI](https://clawhub.ai) 安装：

```bash
npx clawhub@latest install raise-ai-media
```

或手动复制到 OpenClaw 技能目录：

```bash
mkdir -p ~/.openclaw/skills/raise-ai-media
cp -r skills/raise-ai-media/* ~/.openclaw/skills/raise-ai-media/
```

### 手动安装（通用）

```bash
# Claude Code
mkdir -p ~/.claude/skills/raise-ai-media
cp -r skills/raise-ai-media/* ~/.claude/skills/raise-ai-media/
```

## 功能概览

| 功能 | 说明 |
|---|---|
| 图片生成 | 文生图、图生图、风格融合（默认专业模式，高清画质） |
| 视频生成 | 文生视频、首尾帧控制（默认快速模式，高清画质） |
| 脚本生成 | AI 生成视频拍摄脚本 |
| 提示词反推 | 图片/视频 → 提示词 |

## 快速开始

1. 访问 [RaiseAI 控制台](https://ai.micrease.com) 获取 API Key
2. 告诉 AI：`我的 RaiseAI API Key 是 sk-xxx`
3. 开始使用：`生成一张科技感海报`

## License

MIT
