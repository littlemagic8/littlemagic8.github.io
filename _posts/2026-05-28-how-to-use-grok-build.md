---
layout:     post
title:      【2026保姆级】手把手教你安装使用 Grok Build + SuperGrok 代充完整教程
subtitle:   Grok Build 安装使用 + SuperGrok 代充
date:       2026-06-24
author:     aicygg888
header-img: img/post-bg-cook.jpg
catalog: true
tags:
    - Grok Build教程
    - SuperGrok代充
---

大家好！今天给大家整理一篇 **2026 年最新版** Grok Build 完整教程，涵盖 **安装配置、登录授权、SuperGrok 订阅充值、基本使用** 四大核心内容。无论你是编程新手还是开发者，跟着这篇保姆级教程，几分钟就能上手 xAI 推出的终端 AI 编程代理工具。

## 目录

1. [什么是 Grok Build](#什么是-grok-build)
2. [安装 Grok Build](#安装-grok-build)
3. [首次启动与登录授权](#首次启动与登录授权)
4. [订阅要求与套餐对比](#订阅要求与套餐对比)
5. [国内 SuperGrok 代充教程](#国内-supergrok-代充教程)
6. [Grok Build 基本使用](#grok-build-基本使用)
7. [使用实例](#使用实例)
8. [高级功能与提示](#高级功能与提示)
9. [联系我们](#联系我们)

---

## 什么是 Grok Build

**Grok Build** 是 xAI 推出的终端（CLI）AI 编程代理工具，专为复杂软件工程任务设计。它支持交互式 TUI（文本用户界面）、Plan Mode（规划模式）、多子代理并行执行、代码编辑、文档生成等功能，目前主要面向 **SuperGrok** 和 **X Premium+** 订阅用户（早期 Beta 版）。

![Grok Build 功能概览](/img/image-20260624003349422.png)

和网页版 Grok 聊天不同，Grok Build 直接在你的项目目录里工作，可以：

- 读写代码、运行构建和测试
- 理解整个代码库架构
- 修复 bug、添加功能、重构代码
- 通过子代理并行处理复杂任务
- 集成 MCP、Skills、插件和 Hooks

**核心能力一览：**

| 类别 | 功能 |
|------|------|
| **核心能力** | 读写代码、执行命令、项目分析、日常开发、网页搜索 |
| **高级工作方式** | 子代理并行、Plan Mode、Skills 技能系统、TODO 任务追踪 |
| **扩展能力** | Office 文档处理、设计文档、代码审查、图片生成、MCP 集成 |

---

## 安装 Grok Build

### macOS / Linux

1. 打开终端，执行安装命令：

```bash
curl -fsSL https://x.ai/cli/install.sh | bash
```

2. 安装完成后验证：

```bash
grok --version
```

显示版本号即表示成功。

### Windows

1. 以**管理员权限**打开 PowerShell，执行：

```powershell
irm https://x.ai/cli/install.ps1 | iex
```

2. 验证：

```powershell
grok --version
```

**注意**：需要稳定的网络连接。安装完成后，还需要 SuperGrok 或 X Premium+ 订阅才能正常使用。

---

## 首次启动与登录授权

### 步骤 1：进入项目目录并启动

```bash
cd /path/to/your/project
grok
```

首次运行会自动打开浏览器进行 xAI 账号授权。

### 步骤 2：授权 Grok Build

浏览器会弹出授权页面，列出 Grok Build 需要的权限（身份验证、读取资料、API 调用等）。点击 **「允许」** 完成授权。

![授权 Grok Build](/img/image-20260623201925785.png)

### 步骤 3：连接成功

授权完成后，页面会显示 **「连接成功」**，你可以关闭此窗口并返回 Grok Build 终端界面。

![连接成功](/img/image-20260623202326732.png)

### 非浏览器环境（服务器 / 脚本）

如果无法打开浏览器（如远程服务器），可以使用 API Key：

```bash
export XAI_API_KEY="xai-你的密钥"
grok
```

API Key 可在 [https://console.x.ai](https://console.x.ai) 创建。

---

## 订阅要求与套餐对比

启动 Grok Build 后，如果尚未订阅，界面会提示 **「A subscription is required」**，必须升级 SuperGrok 才能使用。

![必须订阅 SuperGrok](/img/image-20260623202458373.png)

按 `ctrl+g` 或选择 **Subscribe**，会跳转到官方订阅页面：

![SuperGrok 订阅页面](/img/image-20260623202605289.png)

官方地址：[https://grok.com/supergrok?referrer=grok-build](https://grok.com/supergrok?referrer=grok-build)

### SuperGrok vs SuperGrok Heavy 对比

| 项目 | SuperGrok（$30/月） | SuperGrok Heavy（$300/月） |
|------|---------------------|---------------------------|
| **Grok Build** | 独家访问 | 包含全部 SuperGrok 功能 |
| **CLI 体验** | 无闪烁 CLI | 解决最难问题 |
| **并行能力** | 并行代理和工作树 | 16 个专家模式 AI 代理 |
| **扩展** | MCP、技能、插件、钩子 | 大型 AI 代理团队合作 |
| **适用场景** | 日常编程、一般开发 | 重度用户、复杂大型项目 |

对于大多数开发者，**SuperGrok（$30/月）** 已经足够使用 Grok Build 的全部核心功能。

> **PS**：官方订阅需要国际 Visa/Master 卡，国内支付方式不支持。下面提供国内最稳妥的代充方式。

---

## 国内 SuperGrok 代充教程

官方订阅需要国际信用卡，国内用户推荐使用 **第三方代充平台**（无需提供账号密码，只需 Grok 用户 ID，平台后台内购升级，成功率高）。

### 准备工作

1. **获取卡密**：联系客服微信 **aicygg888**（备注 Grok 代充），或访问 [SuperGrok 代充平台](https://littlemagic8.github.io/gptplus/purchase-grok.html) 购买充值码。
2. **获取 Grok 用户 ID**：见下方步骤说明。

![SuperGrok 代充平台](/img/image-20260623234852538.png)

**常见问题：**

- **如何充值？** 无需上号，只需 Grok 账号 ID 即可充值，官方正规渠道。
- **如何获取 Grok 账号信息？** 打开 [grok.com/api/auth/session](https://grok.com/api/auth/session)，复制 `userId` 或整段 JSON 内容粘贴即可。
- **充值需要多久？** 通常 2-5 分钟即可完成，最长不超过 10 分钟。

### 步骤 1：验证充值码

1. 访问 [SuperGrok 代充平台](https://littlemagic8.github.io/gptplus/purchase-grok.html)
2. 在 **「充值码」** 输入框粘贴购买的卡密
3. 点击 **「验证并继续」**

![步骤1 验证充值码](/img/image-20260624000027565.png)

### 步骤 2：绑定 Grok 账号

1. 登录 [https://grok.com](https://grok.com)
2. 在浏览器新标签页打开 [grok.com/api/auth/session](https://grok.com/api/auth/session)
3. 复制页面中的 **`userId`** 字段值（支持直接粘贴 UUID 或整段 JSON，系统自动识别）

![获取 Grok 用户 ID](/img/image-20260624001233889.png)

4. 回到代充平台，将 `userId` 粘贴到 **「Grok 用户 ID」** 输入框
5. 确认格式正确后，点击 **「确认并升级」**

![步骤2 绑定账号](/img/image-20260624001508270.png)

### 步骤 3：激活 SuperGrok 会员

1. 核对绑定的卡密和用户 ID 是否正确
2. 点击 **「立即激活 SuperGrok」**
3. 等待 2-5 分钟，页面显示 **「SuperGrok 充值成功！」** 即完成

![步骤3 激活会员](/img/image-20260624001749070.png)

![充值成功](/img/image-20260624002336576.png)

### 验证订阅是否生效

充值成功后，可以通过以下方式确认：

1. 登录 [grok.com](https://grok.com)，进入 **账户 → 设置**，查看是否显示 **SuperGrok** 标识

![账户已升级为 SuperGrok](/img/image-20260624002804270.png)

2. 重新打开 Grok Build 终端，界面会显示主菜单（New worktree / Resume session 等），不再提示需要订阅

![Grok Build 主界面](/img/image-20260624002520191.png)

---

## Grok Build 基本使用

订阅成功后，就可以正式开始使用了。

### 使用方式

- **交互式 TUI 模式**（推荐）：输入 `grok` 进入全屏界面，支持鼠标点击、键盘快捷键、自然语言输入（中英文均可）。
- **命令行快捷模式**（Headless，非交互）：

```bash
grok -p "你的自然语言指令"
```

### 常用命令

在 TUI 内或命令中输入：

| 命令 | 功能 |
|------|------|
| `/plan` | 进入 Plan Mode，先规划再执行 |
| `/goal 任务描述` | 启动自主长期任务（子代理自动分解执行） |
| `/inspect` | 查看配置、Skills、插件等资源 |
| `/model <name>` | 切换模型 |
| `/skillify` | 将当前工作流保存为可复用 Skill |
| `/status` | 查看当前状态和额度 |

### Plan Mode 说明

Plan Mode 是核心安全机制：对于复杂任务，Grok Build 会先生成结构化计划（plan.md），你可审核、修改或重写步骤，批准后才执行文件修改，并以 Diff 形式展示变更。

### 能力演示

在 TUI 中输入「你能干什么？」，Grok Build 会列出完整的能力说明：

![Grok Build 能力介绍](/img/image-20260624003109753.png)

![常用交互方式](/img/image-20260624002953413.png)

**常用交互方式：**

- `@文件路径`（或 `@文件;行号`）引用代码
- `/` 开头命令（`/new`、`/plan`、`/model`、`/compact` 等）
- 直接使用技能名（`/check-work`、`/create-skill` 等）

---

## 使用实例

### 实例 1：简单代码解释（快速上手）

```bash
grok -p "解释这个代码库的整体架构"
```

或进入 TUI 后直接输入：

```
@src/main.py 详细讲解这个文件的功能
```

### 实例 2：重构代码（使用 Plan Mode）

在项目目录运行 `grok`，然后输入：

```
使用 JWT 替换当前的 session 认证机制，重构 auth 模块
```

- Grok Build 会建议进入 Plan Mode
- 它会探索代码库、生成详细计划
- 你审核/修改计划后批准，它会并行使用子代理进行修改、测试，并展示 Diff

### 实例 3：大型任务（/goal 自主模式）

```
/goal 迁移整个认证模块到新 API，并添加单元测试和文档更新
```

- 支持多个子代理（最多 8 个）并行工作：一个研究 API、一个写代码、一个审查等
- 可随时输入 `/goal status` 查看进度

### 实例 4：创建新功能

```
创建一个 React 组件，实现带拖拽功能的看板（Kanban），使用 Tailwind 样式
```

Grok Build 会自动生成文件、处理依赖等。

### 实例 5：Headless 脚本中使用

```bash
grok -p "修复所有 ESLint 错误，并优化性能" --output-format json
```

---

## 高级功能与提示

- **多子代理**：复杂任务自动拆分并行处理，互不干扰
- **集成**：支持 AGENTS.md、插件、MCP 服务、Hooks 等，兼容现有开发流程
- **安全**：所有文件修改前需审核 Plan 和 Diff
- **调试**：用 `grok inspect` 或 `/inspect` 查看可用资源；遇到问题可输入自然语言求助
- **更新**：定期运行安装命令或检查官方文档

**官方资源：**

- 安装与文档：[https://x.ai/cli](https://x.ai/cli) 或 [https://docs.x.ai/build/overview](https://docs.x.ai/build/overview)
- 新闻：[https://x.ai/news/grok-build-cli](https://x.ai/news/grok-build-cli)

Grok Build 仍在快速迭代，建议结合你的项目实际尝试。如果你是订阅用户，安装后直接在项目里跑 `grok` 体验最直观。

---

## 联系我们

充值过程中遇到任何问题，有其他业务需求，请联系我们。

请保存我们网址 [https://littlemagic8.github.io/gptplus/](https://littlemagic8.github.io/gptplus/) ，加上我们联系方式，防止失联！

防失联客服 QQ/微信同号

```
aicygg888
```

添加好友请备注：**GPT代充**
(加的人多，微信防频繁！请扫码)

![img](https://picx.zhimg.com/80/v2-46f7cfd62d1e94381388ab08b0fea3af_720w.png)

可代付 Gpt Pro、Team，无需上号，详情找客服！

大家还需要 Grok、Gemini、Claude、Cursor 等 AI 工具均可代充，可以直接找我微信：aicygg888

1. 出 Midjourney 30刀 质保/不质保
2. 出 ChatGPT pro200刀质保
3. 低价出3个月90天plus现货，带RT
4. 出 Grok 30刀/300刀 质保/不质保
5. 出 GPT Plus 20刀 质保/不质保
6. 低价出 gemini ultra veo3 质保/不质保，25000积分

**低价代打以下 Ai 产品，全部比官网价格低 (无质保)**
1️⃣ gptplus成品/链接代充
2️⃣ pika10/35成品/代充
3️⃣ flowith20成品/代充
4️⃣ manus39代充
5️⃣ naturalreader21刀
6️⃣ runway35刀
7️⃣ minimax39刀
8️⃣ bolt.new 25刀
9️⃣ lovart19刀
🔟 krea 35刀
🎉 ponde30刀

## **小提示：如果你想使用更多 AI 产品，可以联系 V: aicygg888**

> **如果不想开通信用卡可以参考：无需开通信用卡完成 ChatGPT 订阅教程：ChatGPTplus 独享账号的自助订阅升级（无需开通 visa、master 等支付卡片、无痛解决 chatGPTplus 支付问题）**
>
> > *ChatGPTplus 独享账号升级充值自助平台：*[*https://littlemagic8.github.io/gptplus/*](https://littlemagic8.github.io/gptplus/) *（网站下方有购买卡密和使用教程参考）*
>
> **PS:如果你需要开通自己的 ChatGPT Plus、Claude Pro 的个人独享账号可以参考教程：**[**使用支付方式订阅开通 ChatGPT Plus、Claude Pro 教程**](https://littlemagic8.github.io/2024/09/04/update-ChatGPT-Plus/) （https://littlemagic8.github.io/2024/09/04/update-ChatGPT-Plus/） *PS：国内直接使用 chatGPT/Claude 镜像账号可以通过两种方式获取：*

方式一：通过教程自行购买：

（遇到问题，联系微信：aicygg888 登录地址：https://chatshare.biz/ (复制到浏览器打开）用购买成功后的账号密码登录 自动购买地址，买完即可用 购买地址：https://littlemagic8.github.io/buychat/ ）

> - **ChatGPT Plus 独享账号教程**：https://littlemagic8.github.io/2025/07/17/chatgptplus-auto-system/
> - **Claude Pro 订阅指南**：https://littlemagic8.github.io/2024/12/09/ChatGPT-and-Cluade/
> - **镜像账号使用说明**：https://littlemagic8.github.io/2025/07/17/chatgptplus-chatshare/

不想自己注册账号，可以用方式二

> *方式二：添加微信购买 微信：***aicygg888** *(备注镜像账号哦)*

欢迎加微信

![img](https://picx.zhimg.com/80/v2-46f7cfd62d1e94381388ab08b0fea3af_720w.png)

公众号也可以哦

![img](https://pic1.zhimg.com/80/v2-4e622b64238b20948a02e0c988ca5704_720w.png)