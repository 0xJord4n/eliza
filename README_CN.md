# Eliza 🤖

<div align="center">
  <img src="./docs/static/img/eliza_banner.jpg" alt="Eliza Banner" width="100%" />
</div>

<div align="center">

📖 [文档](https://elizaos.github.io/eliza/) | 🎯 [示例](https://github.com/thejoven/awesome-eliza)

</div>

## 🌍 README 翻译

[中文说明](./README_CN.md) | [日本語の説明](./README_JA.md) | [한국어 설명](./README_KOR.md) | [Français](./README_FR.md) | [Português](./README_PTBR.md) | [Türkçe](./README_TR.md) | [Русский](./README_RU.md) | [Español](./README_ES.md) | [Italiano](./README_IT.md) | [ไทย](./README_TH.md) | [Deutsch](./README_DE.md) | [Tiếng Việt](./README_VI.md) | [עִברִית](https://github.com/elizaos/Elisa/blob/main/README_HE.md)

## ✨ 功能

- 🛠️ 全功能的 Discord、Twitter 和 Telegram 连接器
- 🔗 支持所有模型（Llama、Grok、OpenAI、Anthropic 等）
- 👥 多代理和房间支持
- 📚 轻松摄取和交互您的文档
- 💾 可检索的记忆和文档存储
- 🚀 高度可扩展 - 创建您自己的动作和客户端
- ☁️ 支持多种模型（本地 Llama、OpenAI、Anthropic、Groq 等）
- 📦 即插即用！

## 视频教程

[AI Agent Dev School](https://www.youtube.com/watch?v=ArptLpQiKfI&list=PLx5pnFXdPTRzWla0RaOxALTSTnVq53fKL)

## 🎯 使用案例

- 🤖 聊天机器人
- 🕵️ 自主代理
- 📈 业务流程处理
- 🎮 视频游戏 NPC
- 🧠 交易

## 🚀 快速开始

### 先决条件

- [Python 2.7+](https://www.python.org/downloads/)
- [Node.js 23+](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
- [pnpm](https://pnpm.io/installation)

> **Windows 用户注意：** 需要 [WSL 2](https://learn.microsoft.com/en-us/windows/wsl/install-manual)。

### 使用入门模板（推荐）

```bash
git clone https://github.com/elizaos/eliza-starter.git
cd eliza-starter
cp .env.example .env
pnpm i && pnpm build && pnpm start
```

然后阅读[文档](https://elizaos.github.io/eliza/)以了解如何自定义您的 Eliza。

### 手动启动 Eliza（仅推荐给知道自己在做什么的人）

```bash
# 克隆仓库
git clone https://github.com/elizaos/eliza.git

# 检出最新版本
# 该项目迭代速度快，因此我们建议检出最新版本
git checkout $(git describe --tags --abbrev=0)
```

### 使用 Gitpod 启动 Eliza

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/elizaos/eliza/tree/main)

### 编辑 .env 文件

复制 .env.example 到 .env 并填写适当的值。

```
cp .env.example .env
```

注意：.env 是可选的。如果您计划运行多个不同的代理，可以通过角色 JSON 传递密钥。

### 自动启动 Eliza

这将运行所有设置项目并使用默认角色启动机器人。

```bash
sh scripts/start.sh
```

### 编辑角色文件

1. 打开 `packages/core/src/defaultCharacter.ts` 修改默认角色。取消注释并编辑。

2. 要加载自定义角色：
    - 使用 `pnpm start --characters="path/to/your/character.json"`
    - 可以同时加载多个角色文件
3. 连接 X（Twitter）
    - 将角色文件中的 `"clients": []` 更改为 `"clients": ["twitter"]` 以连接 X

### 手动启动 Eliza

```bash
pnpm i
pnpm build
pnpm start

# 项目迭代速度快，有时如果您返回项目需要清理项目
pnpm clean
```

#### 额外要求

您可能需要安装 Sharp。如果启动时出现错误，请尝试使用以下命令安装：

```
pnpm install --include=optional sharp
```

### 社区与联系

- [GitHub Issues](https://github.com/elizaos/eliza/issues)。最佳用途：使用 Eliza 时遇到的错误和功能提案。
- [Discord](https://discord.gg/ai16z)。最佳用途：分享您的应用程序并与社区交流。

## 贡献者

<a href="https://github.com/elizaos/eliza/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=elizaos/eliza" />
</a>

## 星标历史

[![Star History Chart](https://api.star-history.com/svg?repos=elizaos/eliza&type=Date)](https://star-history.com/#elizaos/eliza&Date)