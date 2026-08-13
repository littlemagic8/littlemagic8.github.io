---
layout:     post
title:      永远在线的AI同事Grok Bot上线了！Grok Bot 怎么用？GrokBot 怎么样？如何订阅 SuperGrok Heavy
subtitle:   Grok Bot 上手 + 岗位 Prompt + SuperGrok Heavy 代充
date:       2026-08-13
author:     aicygg888
header-img: img/post-bg-cook.jpg
catalog: true
tags:
    - GrokBot
    - SuperGrok Heavy
    - SuperGrok代充
---

## 前言

![bot-signin-account](/img/2026-08-13-grok46/bot-signin-account.png)

8 月 11 日 xAI 放出新产品 **Grok Bot**：一队永远在线的 AI 同事，有自己的云电脑，能登录你正在用的工具，关笔记本也继续干活。

第二天发布的旗舰模型 **Grok 4.6**（效果、怎么用、怎么订 SuperGrok）这里不展开，看这一篇就行：

> **[Grok 4.6 发布了，效果怎么样？怎么用？](https://littlemagic8.github.io/2026/08/13/how-to-do-use-grok-4.6/)**

本文只讲 Grok Bot：

1. **Grok Bot 是什么、值不值得上**
2. **怎么装、怎么建第一个 Bot、怎么让它 24 小时干活**
3. **国内怎么订阅 SuperGrok Heavy**（Grok Bot 目前卡在 Heavy 这一档）

> **tips：想先用上 Grok 4.6、Grok Build、Imagine，走 SuperGrok（$30）就够；想玩 Grok Bot，必须上 SuperGrok Heavy / Cursor Ultra。**（或者等一等，等等党等GrokBot灰度到SuperGrok）
>
> **充值系统地址**：[https://littlemagic8.github.io/gptplus/purchase-grok.html](https://littlemagic8.github.io/gptplus/purchase-grok.html) （用浏览器打开）
>
> 不会操作或要 订阅SuperGrok/ Heavy / Cursor Ultra，直接微信：**aicygg888** / **aicygg789**（备注：Grok代充）

![Grok Bot 官方视觉](/img/2026-08-13-grok46/01-grokbot-hero.jpg)

---

## 目录

1. [先分清：Grok Bot 不是聊天框](#先分清grok-bot-不是聊天框)
2. [Grok Bot 是什么、值不值得上](#grok-bot-是什么值不值得上)
3. [手把手使用 Grok Bot](#手把手使用-grok-bot)
4. [更好用 Grok Bot 的干货](#更好用-grok-bot-的干货)
5. [套餐怎么选：谁必须上 Heavy](#套餐怎么选谁必须上-heavy)
6. [国内订阅 SuperGrok Heavy](#国内订阅-supergrok-heavy)
7. [常见问题 FAQ](#常见问题-faq)
8. [联系我们](#联系我们)

---

## 先分清：Grok Bot 不是聊天框

| 名字 | 它是什么 | 你在哪用 | 最低门槛 |
| :--- | :--- | :--- | :--- |
| **Grok 4.6** | 新旗舰模型 | grok.com、Cursor、Grok Build、API | SuperGrok $30 就能用，详见 [4.6 那篇](https://littlemagic8.github.io/2026/08/13/how-to-do-use-grok-4.6/) |
| **Grok Bot** | 常驻云电脑的 AI 同事，能登录你的网站/App，关电脑也继续干活 | 桌面端（macOS / Windows）+ iOS | **SuperGrok Heavy**，或 Cursor Ultra / Cursor Teams Premium |
| **SuperGrok / Heavy** | grok.com 官网付费档 | grok.com → 设置 → 订阅 | SuperGrok $30；Plus $100；Heavy 约 $300 |

一句话：

- 只想用最强模型、生图、写代码、Grok Build → **先订 SuperGrok**（[4.6 用法看这篇](https://littlemagic8.github.io/2026/08/13/how-to-do-use-grok-4.6/)）
- 想养一队 24 小时在线的 AI 同事 → **必须 Heavy 或 Cursor Ultra**
- 普通 SuperGrok（$30）和 SuperGrok Plus（$100）**都不带 Grok Bot**

![哪些套餐能开 Grok Bot](/img/2026-08-13-grok46/09-plan-gate.png)

---

## Grok Bot 是什么、值不值得上

![Grok Bot：能真正把活干完的 AI 同事](/img/2026-08-13-grok46/07-grokbot-intro.jpg)

### 它不是又一个聊天框

Grok Bot 是 xAI + Cursor 一起推的新产品（2026-08-11，Early Beta）。官方定义就一句话：

> **一队永远在线的 AI 同事。它们有自己的电脑，会登录你正在用的工具，24 小时接着干。**

和普通 Grok / ChatGPT Agent 最大的差别：

| | 普通聊天 Agent | Grok Bot |
| :--- | :--- | :--- |
| 工作环境 | 你的对话窗口，关了就停 | 云端电脑，关笔记本也继续 |
| 用工具的方式 | 主要靠 API / MCP / 插件 | 能像人一样点网页；有插件更好，没插件也能登 |
| 组织方式 | 一个窗口干所有事 | 每人一个岗位：销售、报销、复现 Bug、参谋 |
| 记忆 | 单次会话为主 | 岗位、偏好、例行流程会沉淀 |
| 协作 | 你当传话筒 | Bot 之间能私信、能拉群 |

xAI 内部已经拿它跑真实业务：销售 Bot 连夜做 outreach，运营 Bot 处理入职和发票，工程 Bot 在产品 UI 里复现 Bug 再把修复交给调试 Bot。

### 真实能力边界

**它现在真能做的：**

- 登录 Gmail / CRM / 分析后台 / 客服系统，把活做到「工具里已经改完」
- 看你演示一遍，存成 Skill / Routine，下次自己跑
- 多个 Bot 并行，一个当参谋分配活
- 桌面和 iPhone 同一条线程接着聊
- 遇到密码、2FA、验证码，把电脑交还给你点一下

**你要接受的限制：**

- Early Beta，可靠性没有第三方大样本评测
- 需要 **SuperGrok Heavy / Cursor Ultra / Cursor Teams Premium**
- 桌面端目前是 macOS + Windows，**没有 Linux**
- 企业要走 waitlist
- 所有 Bot **共用一台云电脑**（登录态、文件、Cookie 是共享的，不是隔离沙箱）
- 额度最高，但不是无限；视频生成尤其容易触顶

### 我的建议：谁该上，谁先别上

**值得上 Heavy / Ultra 的人：**

- 每天有重复的多步工作：早报、CRM 清洗、发票、复现 Bug、竞品巡检
- 已经在用 Cursor Ultra（可能已经自带 Grok Bot，先打开看）
- 需要「关电脑也继续跑」的流程
- 能接受 Beta，先从只读 / 草稿开始，再放开发送和改生产

**先订 SuperGrok $30 就够的人：**

- 主要是聊天、写东西、生图、写代码
- 只想试模型强不强（看 [Grok 4.6](https://littlemagic8.github.io/2026/08/13/how-to-do-use-grok-4.6/)）
- 暂时不需要 24 小时 Agent

Grok Bot 的体验更像「招了一个会点鼠标的同事」，不像「又开了一个更聪明的对话框」。接口本身就在教你怎么派活。

---

## 手把手使用 Grok Bot

官方文档入口：[https://docs.x.ai/grok-bot/get-started](https://docs.x.ai/grok-bot/get-started)

下载 / 开通页：[https://cursor.com/bot/onboarding](https://cursor.com/bot/onboarding)

产品页：[https://x.ai/bot](https://x.ai/bot)

### 0. 开通资格

你需要其中之一：

- SuperGrok Heavy（官网最高档，社区长期报价约 **$300/月**）
- Cursor Ultra（$200/月）
- Cursor Teams Premium（$120/席/月）

用 **Cursor 账号**登录 Grok Bot。如果账号还在 Legacy Privacy Mode，要先改到支持云存储的数据设置，否则 Bot 起不来。

国内没有国际卡，走文末代充最省事。

### 1. 下载安装

打开 [https://x.ai/bot](https://x.ai/bot) 或 [Grok Bot 开通页](https://cursor.com/bot/onboarding)，按电脑下载。

**macOS**

1. 按芯片选 Apple silicon 或 Intel（关于本机 → 看到 Chip 就是苹果芯片）
2. 打开 dmg，把 **Grok Bot** 拖进 Applications
3. 打开时若系统拦截，选「打开」

**Windows**

1. 选 x64 或 Arm64（设置 → 系统 → 关于 → 系统类型）
2. 跑安装包，开始菜单打开 Grok Bot

**iOS**

App Store 搜 **Grok Bot**，和桌面同一账号，同一条对话能两边接着聊。

应用会自动检查更新，也可以在 **Settings → Beta → Check for Updates** 手动更新。

装好打开，就是这块欢迎页：

![Grok Bot 欢迎页，点 Sign in](/img/2026-08-13-grok46/bot-01-signin.jpg)

### 2. 登录和首次引导

1. 欢迎页点 **Sign in**（有的版本写 **Get started**）
2. 浏览器弹出 **Sign in to Grok Bot** 账号页

![Sign in to Grok Bot：Google / GitHub / Apple / 邮箱，或直接 Get access with SuperGrok Heavy](/img/2026-08-13-grok46/bot-signin-account.png)

这里可以：

- 用 **Google / GitHub / Apple** 一键登录
- 填邮箱，点 **使用电子邮件继续**
- 已经订了 SuperGrok Heavy：点 **Get access with SuperGrok Heavy**，用同一套 grok.com 账号绑进去

3. 有的环境会再跳到 **Cursor** 完成授权。登录没完成时，欢迎页会红字提示 `Cursor sign-in did not finish. Try again.`，保持 App 开着再登一次即可

登录成功后会出现三选一：

![登录后选择试用、Ultra 或绑定 SuperGrok Heavy](/img/2026-08-13-grok46/bot-02-signin2.jpg)

| 选项 | 什么时候点 |
| :--- | :--- |
| **Activate Trial** | 先试 7 天（要绑卡，额度很少，很容易用完） |
| **Subscribe Now / Get Ultra** | 直接订 Cursor Ultra $200 |
| **Link Grok Account** | 已经有 **SuperGrok Heavy**，点这里绑定，Bot 就包含了 |

国内没有国际卡、要长期用，走文末代充 Heavy，再到这一步点 **Link Grok Account**。

试用开成功后，**Settings → Usage & Billing** 能看到 7 天试用额度：

![Usage & Billing 里看试用剩余](/img/2026-08-13-grok46/bot-03-pay.jpg)

试用额度很紧，清几封邮件就可能见底。真正要用，还是 Heavy / Ultra：

![试用额度用完会提示 Upgrade](/img/2026-08-13-grok46/bot-09-onboard.jpg)

首次引导会介绍 Bots、共享电脑、Routines，并问你平时用哪些工具。这些回答只影响它推荐第一批同事，**不会自动登录你的 Gmail / Slack**。云电脑在后台准备，最后一页是 **Meet a future teammate**。

### 3. 创建第一个 Bot（别建「万能助手」）

点建议岗位，或自己建：

- **Name**：短、好叫，比如 `Piper`
- **Job**：只写一个主责，比如 `Product performance`
- **Description**：怎么干、用什么、绝对不能干什么

官方示例（可以直接改了用）：

```
Name: Piper
Job: Product performance
Description: 用我们的观测工具查产品性能问题。
保留链接和截图，把证据和猜测分开，先给影响最大的那一条。
永远不要改生产环境配置。
```

好岗位长这样：`Talent Scout`、`Expense Manager`、`Bug Reproduction`、`Weekly Reporter`。

差岗位长这样：`General Helper`、`万能助手`。岗位越糊，它越学不到可复用的习惯。

一个账号最多 **50 个 Bot + 群聊**。用 `Cmd/Ctrl+N` → **Create new agent**。建完后 **Bot actions → Edit Profile** 改名字、头像、职责。

建好后界面像聊天软件：左边是 Bot 列表，中间对话，右边能预览它的云电脑（点名字或 `Cmd/Ctrl+Shift+I` 看全屏）：

![建好 Bot 后：左边对话，右边是它的云电脑屏幕](/img/2026-08-13-grok46/bot-08-cloud-pc.jpg)

### 4. 第一份任务怎么下（五要素）

一份好任务必须写清：

1. **结果**：最后要交什么
2. **来源**：哪些网站、文件、对话
3. **边界**：什么不能做，什么要先问你
4. **交付物**：格式、长度、要不要链接
5. **停手点**：什么时候必须回来等你批

**5 分钟就能看到结果、还不需要登录任何网站的起步任务：**

```
把这份文档总结成 5 条。
另开一节列出所有日期、决策、未决问题。
每条标注页码或章节。
不要改源文件。
```

**第一次让它进真实后台：**

```
打开我们的分析后台，对比本周和新用户激活相对过去 4 周的变化。
找出步骤流失最大的那一级，写一份简短排查计划，带上对应图表链接。
不要改任何 dashboard。
需要登录就叫我接管。
```

真实使用长这样——让它接 Gmail / Calendar，它会自己装插件、叫你点一下授权，然后把明天的安排读回来：

![让 Bot 接上 Gmail 和 Calendar，它自己走完授权再回话](/img/2026-08-13-grok46/bot-04-success.jpg)

### 5. 登录工具：密码和验证码你自己点

Bot 碰到登录页，会请你接管云电脑。比如让它去 Pinterest 找图，它会停在 **Sign in to Pinterest**，对话里出现 **Open computer**：

![需要登录网站时，点 Open computer 自己进去登](/img/2026-08-13-grok46/bot-10-pinterest.jpg)

1. 对话里打开 **Agent Computer** / **Open computer**
2. 点接管
3. **你自己**输入密码、Passkey、2FA、验证码
4. 把控制权还回去

**不要把密码或短信验证码贴进聊天。**

浏览器登录态会留在这台共享电脑上，其他 Bot 之后也能用。有正式插件的服务，优先走 **Settings → Plugins**（左下角 Plugins），比让它点网页稳。

登完它会自己接着干，把结果丢回对话，例如按你的文件名存好图：

![Bot 登录后自己找图、按指定文件名存好交回来](/img/2026-08-13-grok46/bot-11-computer.jpg)

### 6. 看结果、改习惯、存成 Skill / Routine

结果不对，直接改，并写成「以后都这样」：

```
以后周报都用这个格式：5 条要点，链接内嵌，最后一节叫「需要决策」。
把刚才这套流程存成 skill，名字叫 Weekly account health。
```

稳定之后再自动化：

```
每个工作日早上 8:00（北京时间）跑 Daily customer-risk skill。
结果发在这个对话里，带链接。
不要联系客户。
源数据拿不到就报失败，禁止用旧数据凑数。
```

后台 Routine 在笔记本合上后也会跑。先 **Test run**，确认它停在该审批的地方，再打开定时。

---

## 更好用 Grok Bot 的干货

这些是官方文档和最早一批上手的人反复强调的，比「多建几个 Bot」重要。

### 1. 一个 Bot 只负责一个结果

拆分标准：目标不同、工具不同、文风不同、审批边界不同、作息不同，就该拆。

典型小团队（先从 3 个开始，别一上来养 20 个）：

| Bot | 职责 | 审批红线 |
| :--- | :--- | :--- |
| Chief of Staff | 拆活、盯进度、拉群 | 不对外发消息 |
| Researcher | 查资料、做对比、给链接 | 不改任何线上配置 |
| Operator | 进后台执行已批准的动作 | 发送 / 付款 / 删除必须问你 |

### 2. 职责写在 Description，任务写在对话

- Description：`永远不要不经批准发外部邮件`
- 对话：`给这 12 个客户起草跟进`

岗位规则放对话里，下次就会忘。放 Description 里，它会当成长期性格。

### 3. 先做一次，再存 Skill，最后才定时

顺序不要反：

1. 人工盯着跑通一次
2. `Save the process we just used as a skill...`（步骤、校验、输出、审批）
3. 用 **Teach a task** 演示一遍浏览器操作（最长约 10 分钟，不录音频）
4. Test run
5. 再挂日程或 Slack / GitHub 触发器

Skill 要用时，桌面输入框打 `/`；提某个 Bot、群、插件，打 `@`。

### 4. 触发器写窄，别监听「所有新消息」

官方明确警告：太宽的监听又费额度又容易误操作。

```
当 #customer-escalations 里出现工单链接，并且包含 “needs repro”，
打开工单，在 staging 复现，把复现包发回这个对话。
未经批准不要回帖到 Slack。
```

### 5. 共享电脑不是安全边界

所有 Bot 共用：

- 浏览器 Cookie / 登录态
- `/workspace` 文件
- 命令行凭证

所以：

- 不要指望「再建一个 Bot」就能隔离权限
- 敏感临时文件用完删
- 不用的网站记得退出
- 不用的插件去源站撤销授权
- 本地电脑默认 **Ask every time**，没必要就 **Never allowed**

### 6. 审批开关按「会不会花钱 / 会不会发出去」来设

必须人工批：

- 发邮件、发邀请、发社媒
- 付款、转账
- 删除、覆盖数据
- 改生产、改权限
- 点同意法律条款

可以先自动：

- 草稿、对账、推荐、截图、汇总

桌面审批是 **Allow once / Deny / Always allow**。Auto Review 规则写窄，例如「发外部邮件必须批」，不要写「浏览器里什么都允许」。

### 7. 可直接抄的 8 个岗位 Prompt

**早报参谋**

```
每个工作日 8:00 拉日历和未读邮件。
只列今天必须处理的 5 件事，每件给建议动作和原文链接。
不要回复任何邮件。
```

**销售开发**

```
连夜研究这批账户，按意向打分。
按我的口吻起草邮件和 LinkedIn，放进待我审批的草稿箱。
一封都不要发出去。
```

**Bug 复现**

```
打开产品 UI，按工单步骤复现。
交：复现步骤、截图、环境、是否必现。
不要改代码，不要改生产数据。
```

**发票 / 报销**

```
处理 Gmail 里今天的发票。
抽出供应商、金额、日期，放进报销表草稿。
付款和提交必须等我批准。
```

**竞品巡检**

```
每周一打开这 5 个竞品定价页和更新日志。
只报告相对上周的变化，带链接。
不要注册、不要提交表单。
```

**内容日历**

```
根据本周选题，产出 3 条可发的短帖草稿 + 配图说明。
全部放在这个对话里等我改。
不要点发布。
```

**账户健康**

```
拉取产品使用和支持信号，标出流失 / 扩购证据。
给 CS 一份带链接的观察名单。
未经批准不要联系客户、不要改账户。
```

**参谋（管其他 Bot）**

```
你只负责任务拆分和盯进度。
研究类活给 Researcher，执行类活给 Operator。
对外动作一律先汇总给我批。
```

---

## 套餐怎么选：谁必须上 Heavy

以 2026 年 8 月官网公开信息为准。Heavy 的标价不在价格页主卡片上印死，社区和历史档长期按 **约 $300/月** 在谈，偶有促销到 $99 过渡期。下单前以 grok.com 结算页为准。

| 档位 | 大概价格 | Grok Bot | 适合谁 |
| :--- | :--- | :--- | :--- |
| 免费 / SuperGrok Lite | $0～10 | 无 | 试试聊天 |
| **SuperGrok $30** | **$30/月** | **无** | 用模型、Imagine、Grok Build，看 [4.6 那篇](https://littlemagic8.github.io/2026/08/13/how-to-do-use-grok-4.6/) |
| SuperGrok Plus | $100/月 | **无** | 重度生视频 / 怕排队 |
| **SuperGrok Heavy** | **约 $300/月** | **有** | 要 Grok Bot、要先用新功能 |
| Cursor Ultra | $200/月 | **有** | 已经在 Cursor 里写代码 |
| Cursor Teams Premium | $120/席/月 | **有** | 团队账单 / SSO |

选购口诀：

1. **先用模型、生图、写代码** → SuperGrok $30
2. **要 Grok Bot / 抢先体验新功能** → SuperGrok Heavy
3. **已经付了 Cursor Ultra** → 先打开 Grok Bot，别重复再买一份 Heavy
4. 也可以等等，看 Grok Bot 会不会灰度到 SuperGrok

> SuperGrok 不是绝对无限。现在是每周额度池 + Fair Use。普通使用几乎感觉不到墙，连续猛生视频、开超长 Agent 会软限流。触顶后可以买 Extra Credits、开 Auto Top Up，或直接升档。升档通常比反复加油包更划算。

---

## 国内订阅 SuperGrok Heavy

官网要国际 Visa / Master。国内最稳的是 **自助代充**：不用给账号密码，只要 **Grok userId + 卡密**，后台升级。要开 Grok Bot，买 **SuperGrok Heavy**。

### 步骤 1：买 Heavy 充值码

打开自助站（浏览器打开）：

**[https://littlemagic8.github.io/gptplus/purchase-grok.html](https://littlemagic8.github.io/gptplus/purchase-grok.html)**

![SuperGrok 自助充值两步](/img/2026-08-13-grok46/11-purchase.png)

- 要 Grok Bot → 买 **SuperGrok Heavy**
- 只要模型 / 生图 / Grok Build → 买 SuperGrok $30，用法见 [4.6 那篇](https://littlemagic8.github.io/2026/08/13/how-to-do-use-grok-4.6/)
- 不确定买哪档，微信 **aicygg888** 说一下用途即可

### 步骤 2：复制你的 Grok userId

1. 登录 [https://grok.com](https://grok.com)
2. 浏览器打开：[https://grok.com/api/auth/session](https://grok.com/api/auth/session)
3. 复制 `"userId"` 后面那一串，类似 `ea297950-79e4-466a-be73-dd3f8efbd29c`

![复制 Grok userId](/img/2026-08-13-grok46/12-userid.png)

### 步骤 3：回自助站充值

1. 点「第二步：系统充值」
2. 粘贴卡密，再粘贴 userId

![粘贴卡密和 userId](/img/2026-08-13-grok46/13-recharge-step.png)

3. 确认卡密档位是 Heavy，点 **确定并升级**

![绑定账号后确认升级](/img/2026-08-13-grok46/14-recharge-form.png)

4. 等 2～5 分钟
5. 刷新 grok.com，或退出再登录

### 步骤 4：确认到账并打开 Grok Bot

打开 **账户 → 设置 → 订阅**，应看到 **SuperGrok Heavy**。

![在设置里确认订阅到账](/img/2026-08-13-grok46/16-sub-check.png)

没立刻显示时：

- 清缓存 / 无痕再登
- 等几分钟（延迟正常）
- 确认登录的是同一个邮箱
- 还不行就拿 userId 和订单找客服

到账后去 [cursor.com/bot/onboarding](https://cursor.com/bot/onboarding) 下载 Grok Bot，用同一套 Cursor / xAI 登录。

### 官网自己绑卡（有外卡的人）

1. 登录 grok.com
2. 打开 [https://grok.com/supergrok](https://grok.com/supergrok) 或 [价格页](https://x.ai/pricing)
3. 选 Heavy
4. 账单之后在 [https://grok.com/?_s=billing](https://grok.com/?_s=billing) 管理
5. 广告拦截有时会挡住「管理订阅」，换无痕窗口

---

## 常见问题 FAQ

**Q1：Grok Bot 和 grok.com 聊天、Grok Build 是一回事吗？**  
不是。grok.com 是聊天 / 生图；Grok Build 是终端写代码；Grok Bot 是云电脑上的常驻同事。模型怎么用看 [Grok 4.6](https://littlemagic8.github.io/2026/08/13/how-to-do-use-grok-4.6/)。

**Q2：只用模型，必须买 Heavy 吗？**  
不必。SuperGrok $30 就能用 Grok 4.6。Heavy 的关键增量是 **Grok Bot + 最高额度 + 新功能先吃**。

**Q3：Windows 能用 Grok Bot 吗？**  
官方文档写了 Windows 安装（x64 / Arm64）。产品页下载按钮有时只突出 macOS，以 [开通页](https://cursor.com/bot/onboarding) 实际提供的安装包为准。Linux 桌面目前没有。

**Q4：已经有 Cursor Ultra，还要 Heavy 吗？**  
先打开 Grok Bot。Ultra 已包含 Bot。只有还要 grok.com 上最高档 Imagine / 优先队列时，才考虑再叠 Heavy。

**Q5：Grok Bot 会不会乱发邮件、乱改后台？**  
它能做，所以边界要写死。发送、付款、删除、改生产全部要求审批；密码和 2FA 自己点。Beta 阶段先从只读和草稿养。

**Q6：代充安全吗？要不要密码？**  
正规代充只要 userId，不要密码、不要验证码。本站跑了很久，SuperGrok / Heavy 都支持。入口：[purchase-grok.html](https://littlemagic8.github.io/gptplus/purchase-grok.html)

**Q7：订阅后 App 里看不到？**  
确认桌面 / iOS / 网页登录的是同一个 Apple / Google / 邮箱账号。Hide My Email 这类中转邮箱很容易登错号。先退出、清缓存、无痕再登。

**Q8：国内网络怎么访问？**  
需要稳定线路，尽量固定节点，别今天美西明天日本。grok.com 和 X 两套账号可同时用，额度独立。

---

## 总结

| 你的目标 | 现在就做 |
| :--- | :--- |
| 体验模型 / 生图 / 写代码 | 订 SuperGrok，看 [Grok 4.6](https://littlemagic8.github.io/2026/08/13/how-to-do-use-grok-4.6/) |
| 养 24 小时 AI 同事 | SuperGrok Heavy 或 Cursor Ultra，按本文装 Grok Bot |
| 国内付款 | [自助代充](https://littlemagic8.github.io/gptplus/purchase-grok.html) 或微信 aicygg888 |

**一句话：**  
Grok Bot 是另一档产品，第一次让「AI 同事」有自己的电脑和班表。大多数人先上 SuperGrok 吃模型，真正有重复流程再上 Heavy。

---

## 联系我们

充值、选型、Grok Bot 安装卡住，直接找我们。

请先收藏：[https://littlemagic8.github.io/gptplus/](https://littlemagic8.github.io/gptplus/)

自助 SuperGrok / Heavy：[https://littlemagic8.github.io/gptplus/purchase-grok.html](https://littlemagic8.github.io/gptplus/purchase-grok.html)

防失联客服微信：

```
aicygg888
```

也可以加：**aicygg789**

添加请备注：**Grok代充**（加的人多，微信防频繁，优先扫码）

![微信客服](/img/2026-08-02-x-premium-plus/wechat-qr.png)

公众号：

![公众号](/img/v2-4e622b64238b20948a02e0c988ca5704_720w.png)

可代充 / 代付：

1. SuperGrok $30 / SuperGrok Heavy $300（质保 / 不质保）
2. ChatGPT Plus / Pro / Team
3. Claude、Gemini、Cursor Ultra
4. X Premium+
5. Midjourney 及其他常见 AI 工具

**小提示：想用更多 AI 产品，微信 aicygg888**

> 不想自己开国际信用卡，走自助站即可：
>
> [https://littlemagic8.github.io/gptplus/](https://littlemagic8.github.io/gptplus/)
>
> 相关教程：
>
> - [Grok 4.6 效果与用法](https://littlemagic8.github.io/2026/08/13/how-to-do-use-grok-4.6/)
> - [国内订阅 SuperGrok](https://littlemagic8.github.io/2026/04/08/how-to-use-supergrok/)
> - [Grok Build 安装与使用](https://littlemagic8.github.io/2026/06/24/how-to-use-grok-build/)
> - [X Premium+ 订阅](https://littlemagic8.github.io/2026/08/02/how-to-use-X-premium+/)
