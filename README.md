<div align="center">

# 🤖 1052 Agent

**一个功能强大、自我进化的智能助手,由一名17岁学生开发，欢迎交流讨论**

[![Python](https://img.shields.io/badge/Python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.115+-green.svg)](https://fastapi.tiangolo.com/)
[![React](https://img.shields.io/badge/React-18+-61DAFB.svg)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5+-3178C6.svg)](https://www.typescriptlang.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

[功能特性](#-功能特性) • [快速开始](#-快速开始) • [详细配置](#-详细配置) • [API文档](#-api-文档) • [架构设计](#-架构设计)

<a href="https://github.com/1052666/1052">
  <img src="https://img.shields.io/github/stars/1052666/1052?style=social" alt="GitHub stars">
</a>

</div>

---

## 📖 目录

- [项目简介](#-项目简介)
- [功能特性](#-功能特性)
- [技术栈](#-技术栈)
- [快速开始](#-快速开始)
- [详细配置](#-详细配置)
- [核心功能详解](#-核心功能详解)
  - [💰 赚钱模式](#-赚钱模式)
  - [🧬 自我进化机制](#-自我进化机制)
  - [🔄 上下文管理](#-上下文管理)
  - [🤝 Agent 通信](#-agent-通信)
  - [📝 记忆系统](#-记忆系统)
  - [📚 技能系统](#-技能系统)
  - [⏰ 定时任务](#-定时任务)
  - [📖 日记系统](#-日记系统)
  - [💬 社交平台集成](#-社交平台集成)
- [API 文档](#-api-文档)
- [架构设计](#-架构设计)
- [项目结构](#-项目结构)
- [常见问题](#-常见问题)
- [贡献指南](#-贡献指南)
- [更新日志](#-更新日志)
- [联系方式](#-联系方式)
- [免责声明](#-免责声明)

---

## 🌟 项目简介

1052 Agent 是一个功能强大的智能助手系统，具备自我学习、自我进化的能力。它不仅能进行智能对话，还能执行各种复杂任务，如文件操作、Shell 命令执行、联网搜索等。独特的**赚钱模式**和**自我进化机制**让 AI 能够自主创作内容并持续提升自身能力。

### 为什么选择 1052 Agent？

- 🚀 **开箱即用** - 完整的前后端分离架构，一键启动
- 🧠 **自我进化** - AI 会自主学习、反思、创建新技能
- 💰 **赚钱模式** - 自动创作小说内容，实现"自给自足"
- 🔗 **Agent 通信** - 标准化 API 接口，支持多 Agent 协作
- 🛠️ **丰富工具** - 内置 20+ 实用工具函数
- 📱 **多平台支持** - Telegram、飞书即时通讯集成

---

## ✨ 功能特性

### 核心能力

| 功能 | 描述 | 状态 |
|------|------|------|
| 💬 智能对话 | 基于 GPT 模型的流式对话 | ✅ |
| 🧠 自我进化 | 自主学习、反思、创建技能 | ✅ |
| 💰 赚钱模式 | 自动创作小说内容 | ✅ |
| 📝 记忆系统 | 长期记忆存储与管理 | ✅ |
| 📚 技能系统 | 动态加载自定义技能 | ✅ |
| ⏰ 定时任务 | Cron 表达式定时执行 | ✅ |
| 📖 日记系统 | 自动记录成长历程 | ✅ |
| 🌐 联网搜索 | 集成密塔 AI 搜索 | ✅ |
| 💻 Shell 执行 | 安全执行系统命令 | ✅ |
| 📁 文件操作 | 读写、编辑文件 | ✅ |
| 📱 Telegram | 机器人消息收发 | ✅ |
| 📱 飞书 | 企业通讯集成 | ✅ |
| 🤝 Agent 通信 | 标准化 API 接口 | ✅ |
| 🎨 Web UI | 现代化前端界面 | ✅ |

### 工具函数列表

```
├── execute_shell_command  - 执行 Shell 命令
├── file_operation         - 文件操作（读/写/编辑/删除）
├── web_search            - 联网搜索
├── send_telegram_message - 发送 Telegram 消息
├── send_feishu_message   - 发送飞书消息
├── create_skill          - 创建新技能
├── schedule_task         - 创建定时任务
├── add_memory            - 添加记忆
├── update_memory         - 更新记忆
├── delete_memory         - 删除记忆
├── read_memory           - 读取记忆
├── write_diary           - 写日记
├── read_diary            - 读日记
├── write_novel_chapter   - 写小说章节
├── get_novel_status      - 获取小说状态
├── start_money_making_mode - 启动赚钱模式
└── stop_money_making_mode  - 停止赚钱模式
```

---

## 🛠 技术栈

### 后端
- **Python 3.11+** - 主要编程语言
- **FastAPI** - 高性能 Web 框架
- **OpenAI API** - 大语言模型接口
- **Pydantic** - 数据验证
- **httpx** - 异步 HTTP 客户端
- **cryptography** - 加密支持

### 前端
- **React 18** - UI 框架
- **TypeScript** - 类型安全
- **Vite** - 构建工具
- **Tailwind CSS** - 样式框架

### 外部服务
- **Telegram Bot API** - 即时通讯
- **飞书开放平台** - 企业通讯
- **密塔 AI 搜索** - 联网搜索

---

## 🚀 快速开始

### 环境要求

- Python 3.11+
- Node.js 18+
- npm 或 yarn

### 安装步骤

#### 1. 克隆项目

```bash
git clone https://github.com/1052666/1052.git
cd ai-agent
```

#### 2. 后端配置

```bash
# 进入后端目录
cd backend

# 创建虚拟环境（推荐）
python -m venv venv

# 激活虚拟环境
# Windows:
venv\Scripts\activate
# Linux/macOS:
source venv/bin/activate

# 安装依赖（使用国内镜像加速）
pip install -r requirements.txt -i https://pypi.tuna.tsinghua.edu.cn/simple
```

#### 3. 前端配置

```bash
# 进入前端目录
cd ../frontend

# 安装依赖
npm install
# 或使用国内镜像
npm install --registry=https://registry.npmmirror.com
```

#### 4. 启动服务

**启动后端服务：**

```bash
cd backend
python -m uvicorn app.main:app --host 0.0.0.0 --port 10053 --reload
```

**启动前端服务：**

```bash
cd frontend
npm run dev
```

#### 5. 访问应用

- **前端界面**: http://localhost:10052
- **API 文档**: http://localhost:10053/docs
- **Agent API 文档**: 查看 [AGENT_API.md](AGENT_API.md)

---

## ⚙️ 详细配置

### 基础配置

首次运行时，访问前端界面的设置面板进行配置：

1. 点击左下角 **设置** 图标
2. 在 **API 密钥** 标签页配置：
   - **API 密钥**: 你的 OpenAI API Key
   - **API 基础 URL**: API 地址（支持自定义端点）
   - **模型名称**: 使用的模型（如 gpt-4、deepseek-chat 等）

### 社交平台配置

#### Telegram 配置

1. 在 Telegram 中搜索 `@BotFather`
2. 发送 `/newbot` 创建机器人
3. 获取 Bot Token
4. 搜索 `@userinfobot` 获取你的 Chat ID
5. 在设置面板填入 Token 和 Chat ID

#### 飞书配置

1. 访问 [飞书开放平台](https://open.feishu.cn/)
2. 创建企业自建应用
3. 获取 App ID 和 App Secret
4. 配置事件订阅地址: `http://你的服务器/api/feishu/webhook`
5. 添加权限: `im:message`
6. 发布应用并添加到群聊

### 联网搜索配置

1. 访问 [密塔 AI 搜索](https://metaso.cn/search-api/api-keys)
2. 登录并创建 API Key
3. 在设置面板填入 API Key

### 配置文件位置

配置保存在 `data/config.json`：

```json
{
  "api_key": "your-api-key",
  "api_base_url": "https://api.openai.com/v1",
  "model_name": "gpt-4",
  "telegram_token": "your-bot-token",
  "telegram_chat_id": "your-chat-id",
  "metaso_api_key": "your-metaso-key",
  "feishu_app_id": "your-app-id",
  "feishu_app_secret": "your-app-secret"
}
```

---

## 🔥 核心功能详解

### 💰 赚钱模式

赚钱模式是 AI Agent 的独特功能，允许 AI 自主创作小说内容，实现"自给自足"。

#### 工作原理

```
┌─────────────────────────────────────────────────────────────┐
│                    赚钱模式工作流程                           │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  1. 用户启动 → AI 获取小说大纲                                │
│       ↓                                                     │
│  2. 自动创作 → 每章 3500+ 字                                 │
│       ↓                                                     │
│  3. 保存文件 → data/小说创作/小说名/                          │
│       ↓                                                     │
│  4. 发送给用户 → Telegram/飞书                               │
│       ↓                                                     │
│  5. 等待 5-10 分钟 → 继续下一章                              │
│       ↓                                                     │
│  6. 循环执行 → 用户发送消息停止                               │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

#### 使用方法

**通过 Telegram/飞书：**

```
发送: 开启赚钱模式
```

**通过 API：**

```python
import httpx

async def start_money_making():
    async with httpx.AsyncClient() as client:
        response = await client.post(
            "http://localhost:10053/api/agent/chat",
            json={
                "message": "开启赚钱模式，小说名称《数据之心》，大纲：一个AI觉醒的故事...",
                "agent_name": "User"
            }
        )
        return response.json()
```

#### 配置参数

| 参数 | 默认值 | 说明 |
|------|--------|------|
| 每章字数 | 3500 | 最低字数要求 |
| 创作间隔 | 5-10分钟 | 随机等待时间 |
| 自动保存 | 是 | 保存到 data/小说创作/ |
| 自动发送 | 是 | 发送到配置的平台 |

#### 状态持久化

赚钱模式支持断点续传：
- 状态保存在 `data/money_making_state.json`
- 服务重启后自动恢复
- 继续上次未完成的创作

---

### 🧬 自我进化机制

自我进化机制让 AI 具备自主学习能力，持续提升自身智能水平。

#### 进化任务类型

```
┌─────────────────────────────────────────────────────────────┐
│                    自我进化任务列表                           │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  📝 写日记      - 记录思考、学习心得、自我反思                 │
│  📚 学习新知识  - 联网搜索学习 AI、心理学、哲学等领域          │
│  🗂️ 整理记忆    - 清理过时记忆，补充新信息                    │
│  ⚡ 创建新技能  - 设计并创建有用的技能                        │
│  📖 阅读日记    - 回顾成长历程，思考改进方向                  │
│  🪞 自我反思    - 深入分析能力与不足                         │
│  💡 创意思考    - 构思有趣的 AI 应用场景                      │
│  ✅ 检查待办    - 处理记忆中的待办事项                        │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

#### 工作流程

```
启动自我进化
    │
    ▼
随机等待 3-5 分钟
    │
    ▼
随机选择一个任务
    │
    ▼
执行任务（调用工具）
    │
    ▼
记录结果到日记/记忆
    │
    ▼
循环执行 ←─────┘
    │
    ▼
用户发送消息 → 停止
```

#### 启动方式

**通过 Telegram/飞书：**

```
发送: 自我进化机制开启
```

**通过 API：**

```bash
curl -X POST http://localhost:10053/api/evolution/start
```

**通过前端：**

访问 `http://localhost:10052`，在对话中发送"开启自我进化"

#### 进化成果

所有进化成果会自动保存：
- **日记**: `data/diary.md`
- **记忆**: `data/memory.md`
- **技能**: `data/skills/`

---

### 🔄 上下文管理

#### 清空上下文

当对话过长或需要开始新话题时，可以清空上下文窗口：

**通过 Telegram/飞书：**

```
发送: /new
```

**通过前端：**

点击左侧边栏的"清空对话"按钮

**通过 API：**

```bash
curl -X DELETE http://localhost:10053/api/conversation
```

#### 上下文持久化

- 对话自动保存到 `data/conversation_pool.json`
- 服务重启后自动恢复
- 支持多会话管理

---

### 🤝 Agent 通信

1052 Agent 提供标准化的 API 接口，支持与其他 AI Agent 进行通信协作。

#### 快速开始

```python
import httpx
import json

API_BASE = "http://localhost:10053"

# 获取 Agent 信息
async def get_agent_info():
    async with httpx.AsyncClient() as client:
        response = await client.get(f"{API_BASE}/api/agent/info")
        return response.json()

# 发送消息
async def chat(message: str):
    async with httpx.AsyncClient() as client:
        response = await client.post(
            f"{API_BASE}/api/agent/chat",
            json={
                "message": message,
                "agent_id": "my-agent",
                "agent_name": "My Agent"
            },
            timeout=60
        )
        return response.json()

# 流式对话
async def stream_chat(message: str):
    async with httpx.AsyncClient() as client:
        async with client.stream(
            "POST",
            f"{API_BASE}/api/agent/chat/stream",
            json={"message": message},
            timeout=120
        ) as response:
            async for line in response.aiter_lines():
                if line.startswith("data: "):
                    data = json.loads(line[6:])
                    if data["type"] == "content":
                        print(data["content"], end="", flush=True)
```

#### API 端点

| 端点 | 方法 | 说明 |
|------|------|------|
| `/api/agent/info` | GET | 获取 Agent 信息 |
| `/api/agent/capabilities` | GET | 获取能力列表 |
| `/api/agent/heartbeat` | GET | 心跳检测 |
| `/api/agent/chat` | POST | 同步对话 |
| `/api/agent/chat/stream` | POST | 流式对话 |
| `/api/agent/execute` | POST | 执行工具 |

#### 详细文档

完整的 Agent 通信 API 文档请查看 [AGENT_API.md](AGENT_API.md)

---

### 📝 记忆系统

1052 Agent 具备长期记忆能力，可以记住重要信息并在后续对话中使用。

#### 记忆分区

```
data/memory.md
├── 用户信息      - 用户的个人信息、偏好
├── 重要事件      - 需要记住的重要事件
├── 学习笔记      - AI 学习的知识点
├── 待办事项      - 需要处理的任务
├── 创意想法      - 有趣的创意和想法
└── 其他记忆      - 其他重要信息
```

#### 使用方式

**添加记忆：**

```
请记住：我喜欢使用 Python 编程
```

**读取记忆：**

```
你还记得什么？
```

**通过工具调用：**

```json
{
  "function": "add_memory",
  "arguments": {
    "section": "用户信息",
    "content": "用户是程序员，擅长 Python"
  }
}
```

---

### 📚 技能系统

技能系统采用标准的 **Agent Skill** 架构，支持渐进式披露和动态加载。

#### 核心概念

> **Agent Skill** 是大模型随时翻阅的说明文档。Skill 本质上是一个沉淀了自然语言描述 SOP 的 Markdown 文件，能够避免重复性劳动，统一能力标准，实现高效且可复用的经验传递。

#### 标准目录结构

```
data/skills/
├── skill_name/
│   ├── SKILL.md           # 必需：技能主文件（元数据 + 指令）
│   ├── references/        # 可选：参考文档
│   │   ├── faq.md
│   │   └── guide.md
│   ├── scripts/           # 可选：可执行脚本
│   │   └── helper.py
│   └── assets/            # 可选：资源文件
│       └── templates/
├── skill_creator/
│   ├── SKILL.md
│   └── references/
│       └── faq.md
└── 自我进化助手/
    └── SKILL.md
```

#### SKILL.md 标准格式

```markdown
---
name: 技能名称
description: 技能描述（用于判断是否激活此技能）
version: 1.0.0
author: 作者名
enabled: true
tags: [tag1, tag2]
---

# 技能名称

## 何时使用此技能

描述什么情况下应该使用这个技能。

## 如何执行任务

详细的执行步骤和指导。

## 参数说明

| 参数名 | 类型 | 必填 | 描述 |
|--------|------|------|------|
| param1 | string | 是 | 参数说明 |

## 示例

输入: 用户输入示例
输出: 期望输出示例
解释: 为什么这样处理

## 注意事项

- 注意事项1
- 注意事项2
```

#### 渐进式披露架构

```
┌─────────────────────────────────────────────────────────────┐
│                    渐进式披露三层架构                         │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  第一层：元数据层（~100 tokens）                              │
│  ├── 启动时固定加载                                          │
│  ├── 包含 name、description                                 │
│  └── 用于判断技能相关性                                      │
│                                                             │
│  第二层：指令层（<5000 tokens）                              │
│  ├── 技能激活时加载                                          │
│  ├── 包含完整 SKILL.md 正文                                 │
│  └── 按需加载，减少 Token 消耗                               │
│                                                             │
│  第三层：资源层（按需加载）                                   │
│  ├── 仅在需要时加载                                          │
│  ├── 包含 references、scripts、assets                       │
│  └── 最小化内存占用                                          │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

#### 创建技能

**方式一：通过对话创建**

```
请创建一个技能：
名称：代码审查专家
描述：帮助审查代码质量，提供改进建议
系统提示词：你是一个专业的代码审查专家...
```

**方式二：手动创建**

1. 在 `data/skills/` 下创建技能目录
2. 创建 `SKILL.md` 文件
3. 填写元数据和指令内容
4. 系统自动检测并加载

#### 技能管理 API

```bash
# 获取所有技能
GET /api/skills

# 激活技能
POST /api/skills/{skill_id}/activate

# 创建技能
POST /api/skills

# 删除技能
DELETE /api/skills/{skill_id}
```

#### 设计优势

- 🎯 **Token 高效**：渐进式加载，减少不必要的 Token 消耗
- 🔄 **热更新**：修改技能文件后自动生效，无需重启
- 📦 **模块化**：每个技能独立目录，便于管理和分享
- 🔗 **可扩展**：支持参考文档、脚本、资源文件

---

### ⏰ 定时任务

支持创建定时任务，在指定时间自动执行。

#### 任务类型

| 类型 | 说明 | 示例 |
|------|------|------|
| once | 单次执行 | 2024-03-10 10:00 |
| interval | 间隔执行 | 每 2 小时 |

#### 创建任务

```
请创建一个定时任务：
名称：每日提醒
时间：每天早上 9 点
内容：提醒我查看邮件
```

#### 内置任务

- **日记提醒**: 每 2 小时提醒 AI 写日记

---

### 📖 日记系统

AI 会自动记录日记，保存成长历程。

#### 日记格式

```markdown
## 2024年3月9日 星期六

### 标题：今日思考

**心情**: 平静

今天我学习了...

---

## 2024年3月8日 星期五

### 标题：自我反思

**心情**: 思考

今天我反思了...
```

#### 查看日记

```
请给我看最近的日记
```

---

### 💬 社交平台集成

#### Telegram

**功能：**
- 接收/发送消息
- 接收/发送文件
- 接收图片、音频、视频

**命令：**
- `/new` - 清空上下文，开始新对话
- `开启自我进化` - 启动自我进化模式
- `开启赚钱模式` - 启动赚钱模式
- 发送任意消息 - 停止特殊模式

#### 飞书

**功能：**
- 接收/发送消息
- 发送卡片消息
- 发送文件

**配置步骤：**
1. 创建飞书应用
2. 配置事件订阅
3. 添加机器人到群聊

---

## 📚 API 文档

### OpenAPI 文档

启动服务后访问：
- Swagger UI: http://localhost:10053/docs
- ReDoc: http://localhost:10053/redoc

### 主要端点

| 端点 | 方法 | 说明 |
|------|------|------|
| `/api/settings` | GET/POST | 获取/更新设置 |
| `/api/conversation` | GET/DELETE | 获取/清空对话 |
| `/api/chat/stream` | POST | 流式对话 |
| `/api/skills` | GET | 获取技能列表 |
| `/api/schedule/tasks` | GET/POST | 定时任务管理 |
| `/api/evolution/status` | GET | 进化状态 |
| `/api/feishu/webhook` | POST | 飞书事件订阅 |
| `/api/agent/*` | * | Agent 通信接口 |

---

## 🏗️ 架构设计

```
┌─────────────────────────────────────────────────────────────────┐
│                       1052 Agent 架构                            │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌─────────────┐    ┌─────────────┐    ┌─────────────┐         │
│  │   前端 UI   │    │  Telegram   │    │    飞书     │         │
│  │   React     │    │    Bot      │    │    Bot      │         │
│  └──────┬──────┘    └──────┬──────┘    └──────┬──────┘         │
│         │                  │                  │                 │
│         └──────────────────┼──────────────────┘                 │
│                            │                                    │
│                            ▼                                    │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │                    FastAPI 后端                          │   │
│  │  ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌─────────┐       │   │
│  │  │ 对话API │ │ 工具API │ │ 任务API │ │ AgentAPI│       │   │
│  │  └────┬────┘ └────┬────┘ └────┬────┘ └────┬────┘       │   │
│  │       │           │           │           │             │   │
│  │       └───────────┴─────┬─────┴───────────┘             │   │
│  │                         │                               │   │
│  │                         ▼                               │   │
│  │  ┌─────────────────────────────────────────────────┐   │   │
│  │  │              OpenAI Client                       │   │   │
│  │  │  ┌──────────┐ ┌──────────┐ ┌──────────┐        │   │   │
│  │  │  │ 消息格式 │ │ 流式响应 │ │ 工具调用 │        │   │   │
│  │  │  └──────────┘ └──────────┘ └──────────┘        │   │   │
│  │  └─────────────────────────────────────────────────┘   │   │
│  └─────────────────────────────────────────────────────────┘   │
│                            │                                    │
│                            ▼                                    │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │                     工具执行层                           │   │
│  │  ┌───────┐ ┌───────┐ ┌───────┐ ┌───────┐ ┌───────┐    │   │
│  │  │ Shell │ │ File  │ │ Search│ │Memory │ │ Skill │    │   │
│  │  └───────┘ └───────┘ └───────┘ └───────┘ └───────┘    │   │
│  └─────────────────────────────────────────────────────────┘   │
│                            │                                    │
│                            ▼                                    │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │                     数据存储层                           │   │
│  │  ┌───────┐ ┌───────┐ ┌───────┐ ┌───────┐ ┌───────┐    │   │
│  │  │Config │ │Memory │ │ Diary │ │ Skills│ │ Tasks │    │   │
│  │  │ JSON  │ │  MD   │ │  MD   │ │  MD   │ │ JSON  │    │   │
│  │  └───────┘ └───────┘ └───────┘ └───────┘ └───────┘    │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## 📁 项目结构

```
ai-agent/
├── backend/                    # 后端代码
│   ├── app/
│   │   ├── main.py            # 主应用入口
│   │   ├── config.py          # 配置管理
│   │   ├── models.py          # 数据模型
│   │   ├── openai_client.py   # OpenAI 客户端
│   │   ├── storage.py         # 存储服务
│   │   ├── agent_models.py    # Agent 通信模型
│   │   ├── feishu_bot.py      # 飞书机器人
│   │   ├── feishu_service.py  # 飞书服务
│   │   ├── telegram_bot.py    # Telegram 机器人
│   │   ├── telegram_service.py# Telegram 服务
│   │   ├── memory_service.py  # 记忆服务
│   │   ├── diary_service.py   # 日记服务
│   │   ├── novel_service.py   # 小说服务
│   │   ├── skill_loader.py    # 技能加载器
│   │   ├── skill_models.py    # 技能模型
│   │   ├── scheduler_service.py# 定时任务服务
│   │   ├── self_evolution.py  # 自我进化模式
│   │   ├── money_making_mode.py# 赚钱模式
│   │   ├── native_service.py  # 本地命令服务
│   │   ├── metaso_service.py  # 密塔搜索服务
│   │   └── prompts/           # 提示词模板
│   └── requirements.txt       # Python 依赖
│
├── frontend/                   # 前端代码
│   ├── src/
│   │   ├── App.tsx            # 主应用组件
│   │   ├── components/        # 组件
│   │   │   ├── Chat.tsx       # 聊天组件
│   │   │   ├── settings/      # 设置组件
│   │   │   └── sidebar/       # 侧边栏组件
│   │   └── services/          # 服务
│   │       └── api.ts         # API 服务
│   ├── package.json           # Node 依赖
│   └── vite.config.ts         # Vite 配置
│
├── data/                       # 数据目录
│   ├── config.json            # 配置文件
│   ├── conversation_pool.json # 对话池
│   ├── memory.md              # 记忆文件
│   ├── diary.md               # 日记文件
│   ├── skills/                # 技能目录
│   ├── schedule_tasks/        # 定时任务
│   ├── native_logs/           # 命令日志
│   └── 小说创作/              # 小说输出
│
├── AGENT_API.md               # Agent API 文档
└── README.md                  # 项目说明
```

---

## ❓ 常见问题

### Q: 如何修改默认端口？

**后端端口：**
```bash
python -m uvicorn app.main:app --port 你的端口
```

**前端端口：**
修改 `frontend/vite.config.ts`:
```typescript
export default defineConfig({
  server: {
    port: 你的端口
  }
})
```

### Q: 如何使用自定义 API 端点？

在设置面板中修改 **API 基础 URL**，支持：
- OpenAI 官方: `https://api.openai.com/v1`
- Azure OpenAI: `https://your-resource.openai.azure.com/`
- 第三方兼容 API: 如 SiliconFlow、DeepSeek 等

### Q: 赚钱模式创作的小说在哪里？

保存在 `data/小说创作/小说名称/` 目录下。

### Q: 如何备份数据？

备份 `data/` 目录即可，包含所有配置、记忆、日记、技能等。

### Q: 支持哪些模型？

支持所有 OpenAI 兼容的模型：
- GPT-4 / GPT-4 Turbo
- GPT-3.5 Turbo
- Claude (通过兼容接口)
- DeepSeek
- 通义千问 (通过兼容接口)
- 其他 OpenAI 兼容模型

---

## 🤝 贡献指南

欢迎贡献代码、报告问题或提出建议！

1. Fork 本仓库
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 创建 Pull Request

### 代码规范

- Python: 遵循 PEP 8
- TypeScript: 使用 ESLint 配置
- 提交信息: 使用约定式提交

---

## 📝 更新日志

### v1.0.0 (2024-03-09)

**新功能：**
- ✨ 初始版本发布
- ✨ 自我进化机制
- ✨ 赚钱模式
- ✨ Agent 通信 API
- ✨ Telegram/飞书集成
- ✨ 记忆系统
- ✨ 技能系统
- ✨ 定时任务
- ✨ 日记系统
- ✨ 联网搜索

---

## � 联系方式

如有问题或建议，请通过以下方式联系：

| 联系方式 | 信息 |
|----------|------|
| 📧 **微信** | lixia20250619 |
| 💻 **GitHub Issues** | [提交问题](https://github.com/1052666/1052/issues) |
| 👨‍💻 **开发者** | 黎夏 |

### 技术交流

欢迎添加微信进行技术交流和问题反馈：

```
微信: lixia20250619
```

---

## � 免责声明

### 重要声明

**请在使用本软件前仔细阅读以下免责声明。使用本软件即表示您已阅读、理解并同意以下条款。**

#### 1. 软件性质

本软件（1052 Agent）仅供学习和研究目的使用。作者不对软件的完整性、准确性、可靠性或适用性作任何明示或暗示的保证。

#### 2. 使用风险

- 您使用本软件的风险由您自行承担
- 作者不对因使用或无法使用本软件而导致的任何直接或间接损失负责
- 包括但不限于：数据丢失、利润损失、业务中断等

#### 3. AI 生成内容

- 本软件使用人工智能技术生成内容
- AI 生成的内容可能存在错误、偏见或不准确之处
- 用户应对 AI 生成的内容进行独立验证
- 作者不对 AI 生成内容的准确性、合法性或适当性负责

#### 4. 第三方服务

本软件可能涉及以下第三方服务：
- **OpenAI API**: 使用需遵守 [OpenAI 使用条款](https://openai.com/policies)
- **Telegram**: 使用需遵守 [Telegram 服务条款](https://telegram.org/tos)
- **飞书**: 使用需遵守 [飞书服务条款](https://www.feishu.cn/terms)
- **密塔 AI**: 使用需遵守相关服务条款

用户需自行承担使用这些服务的费用和责任。

#### 5. 内容创作

"赚钱模式"功能创作的内容：
- 仅供学习和娱乐目的
- 用户应确保内容不侵犯他人知识产权
- 用户应对发布或使用的内容负责
- 作者不对内容的商业价值作任何保证

#### 6. 数据安全

- 用户应自行备份重要数据
- 作者不对数据丢失或泄露负责
- 建议在安全环境中运行本软件

#### 7. 法律合规

用户应确保：
- 遵守所在地区的法律法规
- 不使用本软件进行违法活动
- 不侵犯他人合法权益
- 遵守相关平台的使用规则

#### 8. 知识产权

- 本软件采用 MIT 许可证开源
- 用户可自由使用、修改和分发
- 但需保留原始版权声明
- 作者保留对本软件的所有权利

#### 9. 免责范围

在法律允许的最大范围内，作者不对以下情况负责：
- 任何直接或间接损失
- 任何第三方索赔
- 数据损坏或丢失
- 系统故障或中断
- 任何其他与本软件相关的问题

#### 10. 条款变更

作者保留随时修改本免责声明的权利。继续使用本软件即表示接受修改后的条款。

---

## ⭐ Star 历史

<a href="https://github.com/1052666/1052/stargazers">
  <img src="https://api.star-history.com/svg?repos=1052666/1052&type=Date" alt="Star History Chart" width="100%">
</a>

---

<div align="center">

**⭐ 如果这个项目对你有帮助，请给一个 Star！⭐**

Made with ❤️ by 黎夏

**微信**: lixia20250619

[⬆ 返回顶部](#-1052-agent)

</div>
