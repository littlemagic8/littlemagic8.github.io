---
layout:     post
title:      Grok 4.6 发布了，效果怎么样？怎么用？如何订阅 SuperGrok / Heavy
subtitle:   Grok 4.6 实测 + 用法干货 + SuperGrok / Heavy 代充
date:       2026-08-13
author:     aicygg888
header-img: img/post-bg-cook.jpg
catalog: true
tags:
    - Grok4.6
    - SuperGrok Heavy
    - SuperGrok代充
    - Grok Build
---

8 月 12 日 xAI 连发旗舰模型 **Grok 4.6**。前一天刚出的新产品 **Grok Bot**（24 小时在线的 AI 同事）单独写了一篇，需要的看这里：

> **[Grok Bot 怎么用？值不值得上 SuperGrok Heavy？](https://littlemagic8.github.io/2026/08/13/how-to-do-use-grok-bot/)**

本文只讲模型本身：

1. **Grok 4.6 到底强在哪、弱在哪**
2. **怎么把它用在 grok.com / Cursor / Grok Build / API 里**
3. **国内怎么订阅 SuperGrok / SuperGrok Heavy**

> **tips：想先用上 Grok 4.6、Grok Build、Imagine，走 SuperGrok（$30）就够；想玩 Grok Bot，必须上 SuperGrok Heavy / Cursor Ultra。**（或者等一等，等等党等GrokBot灰度到SuperGrok）
>
> **充值系统地址**：[https://littlemagic8.github.io/gptplus/purchase-grok.html](https://littlemagic8.github.io/gptplus/purchase-grok.html) （用浏览器打开）
>
> 不会操作或要 订阅SuperGrok/ Heavy / Cursor Ultra，直接微信：**aicygg888** / **aicygg789**（备注：Grok代充）

![grok.com SuperGrok 主界面](/img/2026-08-13-grok46/10-grok-home.png)

---

## 目录

1. [先把三样东西分清](#先把三样东西分清)
2. [Grok 4.6 效果怎么样](#grok-46-效果怎么样)
3. [Grok 4.6 怎么用](#grok-46-怎么用)
4. [看看大家怎么用 Grok 4.6 更好的干活](#看看大家怎么用-grok-46-更好的干活)
5. [套餐怎么选：SuperGrok 还是 Heavy](#套餐怎么选supergrok-还是-heavy)
6. [国内订阅 SuperGrok / SuperGrok Heavy](#国内订阅-supergrok--supergrok-heavy)
7. [常见问题 FAQ](#常见问题-faq)
8. [联系我们](#联系我们)

---

## 先把三样东西分清

很多人把 Grok、Grok 4.6、Grok Bot 混成一谈。先记住这张表：

| 名字 | 它是什么 | 你在哪用 | 最低门槛 |
| :--- | :--- | :--- | :--- |
| **Grok 4.6** | 新旗舰模型，擅长长任务、写代码、做知识工作、出第一版产品 | grok.com、Cursor、Grok Build、API | SuperGrok $30 就能用；首周 Cursor / Grok Build 还有 **2 倍额度** |
| **Grok Bot** | 常驻云电脑的 AI 同事，能登录你的网站/App，关电脑也继续干活 | 桌面端（macOS / Windows）+ iOS | **SuperGrok Heavy**，或 Cursor Ultra / Cursor Teams Premium |
| **SuperGrok / Heavy** | grok.com 官网付费档 | grok.com → 设置 → 订阅 | SuperGrok $30；Plus $100；Heavy 约 $300 |

一句话：

- 只想用最强模型、生图、写代码、Grok Build → **先订 SuperGrok**
- 想养一队 24 小时在线的 AI 同事 → **必须 Heavy 或 Cursor Ultra**（详见 [Grok Bot 教程](https://littlemagic8.github.io/2026/08/13/how-to-do-use-grok-bot/)）
- 普通 SuperGrok（$30）和 SuperGrok Plus（$100）**都不带 Grok Bot**

官网主入口仍然是 **[https://grok.com](https://grok.com)**。和 X（推特）上的 Grok 是两套额度，互不影响。

---

## Grok 4.6 效果怎么样

### 官方定位

xAI 自己的说法很明确：Grok 4.6 不是再堆一个更大参数的模型，而是在 4.5 之上专门补了两块：

- **长程 Agent**：研究陌生领域、翻代码库、多步工具调用，不容易半路跑偏
- **更敢做视觉 / 交互产品**：给一个产品想法，它能一次搭出结构、交互和视觉语言，再按反馈迭代

官方测试里，它特别擅长「把一个很复杂的想法做成能跑的第一版」：先调研，再拆结构，再实现核心交互，然后自己测、自己改。

> Grok4.6刚出来，马斯克就在给Grok4.7造势了！说Grok4.7将成为最强的AI大模型！！
>
> 当然我自己现在的博文很大部分都是由GrokBuild润色的，速度快，效果还不错~ 
>
> 想要安装使用GrokBuild教程可参考：[https://littlemagic8.github.io/2026/06/24/how-to-use-grok-build/](https://littlemagic8.github.io/2026/06/24/how-to-use-grok-build/) (使用浏览器打开)

### 跑分：回到第一梯队，而且便宜

独立评测站 Artificial Analysis 的结论更直白：

- **Intelligence Index = 61**，和 GPT-5.6 Sol 持平
- 只落后 Claude Opus 5（63）和 Claude Fable 5（62）
- 比一个月前的 Grok 4.5 高 5 分，比 4.3 高 23 分
- 上下文仍是 **50 万 tokens**
- API 价没涨：**输入 $2 / 百万 tokens，输出 $6 / 百万 tokens**
- 单任务成本约 **$0.84**，比 Opus / Sol 便宜一大截

![Grok 4.6 在 Artificial Analysis Intelligence Index 上回到第一梯队](/img/2026-08-13-grok46/03-aa-intelligence.png)

xAI / Cursor 放出的对照表也值得看一眼：

![Grok 4.6 官方评测对照](/img/2026-08-13-grok46/02-grok46-evals.png)

用人话翻译这张表：

| 能力 | Grok 4.6 表现 | 你该怎么理解 |
| :--- | :--- | :--- |
| 综合智力 | 61，对齐 GPT-5.6 Sol | 日常推理、写作、研究已经是第一梯队 |
| 知识工作 Agent（GDPVal） | 1753，仅次于 Opus 5 | 调研、写材料、做分析很能打 |
| 写代码 / 改仓库 | CursorBench 69.9%，DeepSWE 65.9% | 写应用、改现有项目很强；硬核底层题还略逊 Sol / Fable |
| 长任务效率 | AA-Briefcase 1577，平均约 53 轮就收工 | 同样一件事，它比 Opus 少转很多圈，更省钱 |
| 法律 / 专业卷面（Harvey LAB） | 15.8%，表里最高 | 正式文书、专业分析第一稿更像样 |

性价比是它真正吓人的地方：智力几乎贴着 Sol，价格却只有它的一小半。

![智力 vs 单任务成本：Grok 4.6 落在更划算的区间](/img/2026-08-13-grok46/05-aa-cost.png)

### 真实体感（Cursor 内部实测）

Cursor 工程师 Eric Zakariasson 把 4.6 当了几周主力，结论很具体，比跑分更有用：

1. **沟通密度高、速度快**。过程摘要是信息，不是把你的任务复读一遍。
2. **适合「边看边改」**。4.5 已经快，4.6 是「又快又聪明」，所以更适合小步同步，而不是一次甩一份超长需求然后干等。
3. **第一版成品明显更好看**。同样让它做浏览器策略游戏，4.5 给的是扁平原型，4.6 第一次就做出等距 3D、HUD 和小地图。
4. **会自己点开页面验收**。你只要加一句「打开应用、按真实用户路径点一遍、检查公式/交互、再修」，质量会跳一档。
5. **别迷信「work very hard」这类空话**。几乎没用。真正有用的是：写清「什么叫做完」。

一句话评价：

> Grok 4.6 不是某一项碾压全世界，而是「写代码、做调研、点网页、出第一版产品」都够强，而且快、便宜、能自己验收。适合当默认主力，而不是只拿来刷题。

![Grok 4.6 与 4.5 / GPT-5.6 / Fable 5 的定位](/img/2026-08-13-grok46/06-grok46-vs.jpg)

---

## Grok 4.6 怎么用

Grok 4.6 现在有 4 条正经入口。按你的场景选就行。

### 路线 1：普通用户 / 创作者 → grok.com（最推荐）

适合聊天、DeepSearch、Imagine 生图/视频、写小说、做方案。

1. 打开 [https://grok.com](https://grok.com)，用邮箱注册（QQ / 163 / Gmail 都行）。
2. 登录后在模型选择里切到 **Grok 4.6**（或 Auto，高峰时 SuperGrok 会优先排队）。
3. 需要生图 / 视频，点右上角 **Imagine**。
4. 额度看 **设置 → Usage**。2026 年 6 月后付费档改成「每周共享额度池」，聊天、Imagine、Voice、Build 共用一桶算力。

免费档现在基本只能轻度聊天。生图、视频、长推理、Grok Build 都在付费墙后面。日常创作用 SuperGrok（$30）性价比最高。

### 路线 2：写代码 → Cursor（首周 2 倍额度）

1. 打开 [https://cursor.com](https://cursor.com)，登录。
2. 模型选择器里选 **Grok 4.6**。
3. 首周官方送 **2x included usage**，适合拿真实项目压测。
4. 适合：从想法做出第一版 App、跨仓库改 bug、边写边在浏览器里点一点做 QA。

### 路线 3：终端 Agent → Grok Build

Grok Build 是 xAI 自己的终端编程代理，对标 Claude Code / Codex。SuperGrok 就能用。

macOS / Linux：

```bash
curl -fsSL https://x.ai/cli/install.sh | bash
grok --version
```

Windows（管理员 PowerShell）：

```powershell
irm https://x.ai/cli/install.ps1 | iex
grok --version
```

然后进入项目目录：

```bash
cd /path/to/your/project
grok
```

首次会弹出浏览器授权。授权后就能在仓库里改代码、跑测试、开 Plan Mode、派子代理。

![Grok Build 能力概览](/img/2026-08-13-grok46/17-grok-build.png)

更细的安装步骤可以看我们之前的教程：[Grok Build 保姆级教程](https://littlemagic8.github.io/2026/06/24/how-to-use-grok-build/)。

### 路线4：开发者 → API / OpenRouter

- 控制台：[https://console.x.ai](https://console.x.ai)
- 模型名：`grok-4.6`
- 价格：$2 / $6（每百万 tokens），有更快的 fast 变体，价格翻倍
- 也上了 OpenRouter、Vercel、Cloudflare
- 知识截止日期：2026-02-01（实时信息要开联网 / X 搜索）

### 首周怎么白嫖一波

xAI 给 Cursor 和 Grok Build 开了 **第一周 2 倍包含额度**。最划算的试法：

1. 订好 SuperGrok
2. 在 Cursor 或 Grok Build 里切到 Grok 4.6
3. 别拿「写个 Hello World」试，直接丢一个真实任务：
   - 把一个产品想法做成能点的第一版
   - 在现有仓库里修一个跨文件 bug
   - 调研一个你不熟的领域，交一份带出处的简报

---

## 看看大家怎么用 Grok 4.6 更好的干活

空技巧没人愿意订。下面 6 个都是这几天已经落地的活：有人用它出了能玩的第一版、有人直接做出开源产品、有人把别人修不通的演示给救回来。每个例子后面都跟了**可复制提示词**，SuperGrok 开通当天就能照着跑。

### 例子 1：一句话做出「能玩」的第一版产品

Cursor 工程师 Eric Zakariasson 把 4.6 当了几周主力，专门拿难项目压：

| 项目 | 4.5 给的 | 4.6 第一次给的 | 你能套用的场景 |
| :--- | :--- | :--- | :--- |
| 浏览器版《帝国时代 2》 | 能玩的扁平原型 | 等距 3D、HUD、小地图、战争迷雾都在 | 小游戏 / 互动落地页 / Demo |
| MSN Messenger 复刻 | 能认出是 MSN | 独立聊天窗、眨眼动画，更像真的 | 怀旧站、品牌互动页 |
| 在线表格 App | 两页规格 vs 三句话，成品差不多 | 加上「自己点开验收」后质量跳一档 | 内部工具、后台、SaaS 骨架 |
| 给开源白板加「演示模式」 | 功能能落地 | 第一轮细节更齐，少改几轮 | 在现有仓库里加功能 |
| 60～90 秒发布片（Remotion，视频当代码写） | 能成片 | 节奏和故事更完整 | 产品发布、短视频脚本落地 |

他的结论很实在：4.6 不是某一项碾压，而是**第一版就完整、会自己点网页验收、适合坐在旁边边看边改**。免费档额度根本撑不住这种长任务，这正是 SuperGrok 值 $30 的地方。

**照抄提示词（Cursor / Grok Build）：**

```
做一个浏览器里能直接玩的 [产品]，新用户 10 秒看懂。
必须有：主路径、空状态、错误提示、移动端还能点。
不要先写文档，直接出能打开的版本。
做完后你自己启动预览，按真实用户路径点一遍：
注册/开始 → 核心操作 → 保存 → 刷新还在。
把点到的问题和修复列出来。没验证过的不要写「已完成」。
```

---

### 例子 2：用 4.6 直接做出能上线的开源产品

Inbox 产品 Inbox Zero 的作者 Elie Steinbock，用 **Cursor + Grok 4.6** 做出了开源项目 **Rakazo**：Web / 桌面 / 手机三端、可自托管的「AI 同事」——本质是 Grok Bot 的开源替代。他自己评价：*It's a nice model.*

![用 Cursor + Grok 4.6 做出来的 Rakazo](/img/2026-08-13-grok46/19-rakazo.jpg)

这类活的共同点：页面多、状态多、还要像真人同事一样派活。4.6 擅长一次立住信息架构和视觉语言，再按反馈改，比你自己从零搭脚手架快一个数量级。

**照抄提示词：**

```
做一个「AI 同事」桌面 App 的第一版：
左侧是多个 Bot 岗位列表，中间是对话，右侧能看 Bot 正在操作的电脑。
先做 Inbox Manager 这一个岗位：归档广告、起草回复、把需要我拍板的标红。
技术栈你定，但要能本地跑起来。
做完打开页面走一遍：建 Bot → 发任务 → 看到草稿。截图给我。
```

---

### 例子 3：别人做不出来的演示，4.6 修通了

中文创作者岚叔同一天拿 DeepSeek V4 Pro 和 Grok 4.6 对打。总体互有胜负，但他点出一个很能说明问题的细节：

> 施瓦西黑洞，V4 Pro 开发完展示不出来，最后是 4.6 给修好的。总体感觉 Grok 4.6 更快、更全面些。

这就是 4.6 的典型价值：**不是只会写代码，还会把「跑不起来 / 看不见」这条最后一公里补上**。免费试用最容易卡在这里——额度一到，验收和返工就停了。

**照抄提示词：**

```
用 WebGL / Three.js 做一页 [可视化演示]，打开就能转、能缩放。
做完你自己在浏览器里打开：
1）画布不是黑的
2）交互能用
3）把控制台报错修掉
修不通就换实现，不要丢一个打不开的 HTML 给我。
```

---

### 例子 4：收件箱从 200 封收成「只剩要回的几封」

还是 Eric 的日常，不是演示项目：

- 邮件收到只剩真正要回的几封
- 自己点开服务商后台申请 API Key（没有现成 API 也能点网页）
- 对正在跑的 App 做功能和视觉 QA

这些是 SuperGrok 在 grok.com 里就能干的「上班活」，不用写代码。

**照抄提示词（grok.com，打开联网）：**

```
这是我今天的邮件/待办摘录：
[粘贴]
请只保留今天必须处理的 5 件事。
每件给：一句话原因、建议回复草稿、要不要我本人出面。
广告、订阅、已读回执全部丢掉。
不确定的单独列，不要装懂。
```

---

### 例子 5：季报 PPT 不再是「把数字糊上幻灯片」

Eric 拿同一份虚构季报让 4.5 和 4.6 做董事会材料：分析能力差不多，差在呈现——4.5 像数据堆砌，4.6 有层级、有结构，读起来像人做的。Harvey LAB 法律卷面那项 4.6 也是对照表里最高的，同一类能力。

**照抄提示词：**

```
根据下面数据和口径，做一份 8 页董事会材料大纲（可直接贴到 PPT）：
[粘贴本月数字 / 表格]
要求：封面结论先行；每页一个判断 + 一个证据；最后一页只要 3 个决策题。
不要堆表。数字对不上就标红，不要编。
```

国内写周报、写方案、给客户出一版「能上会」的稿，这是 SuperGrok 最容易当天回本的用法。

---

### 例子 6：看图、数东西，4.5 到 4.6 是断档式提升

计算机视觉公司 Roboflow 用真实硬币照片测目标检测：同样 8 个物体，**Grok 4.5 的 mAP@50 只有 12.5%，4.6 到了 87.5%**。框更贴、数量也对了。

![Roboflow：Grok 4.5 vs 4.6 目标检测](/img/2026-08-13-grok46/18-roboflow-vision.jpg)

对做电商主图质检、表格/截图抽数、漫画分镜、设计验收的人，这是能直接省人工的能力。免费档生图/看图额度几乎没有，付费之后才谈得上批量用。

**照抄提示词（grok.com 上传图片）：**

```
数图里的 [物体]，每个给：类别、大概位置、有没有被挡住。
再列 3 条质检问题（模糊、裁切、光线）。
不确定的单独标，不要猜。
```

---

### 这 6 个例子，共同值多少钱？

| 你平时在干的 | 4.6 替你拿下的 | 更合适的档 |
| :--- | :--- | :--- |
| 出 Demo / 小工具 / 落地页 | 第一版就能点，少改三轮 | SuperGrok $30 |
| 写周报、方案、客户材料 | 有结构、有结论，不是粘表 | SuperGrok $30 |
| 清邮件、点后台、做 QA | 关聊天框前就能交差 | SuperGrok $30 |
| 漫画 / 主图 / 质检 / 看图抽数 | 识别明显准一档 | SuperGrok（生图再加额度） |
| 连续开超长 Agent、先吃新功能 | 额度更高、Grok Bot | SuperGrok Heavy |

> 想今晚就复现例子 1～5：先开通 SuperGrok，去 grok.com 或 Cursor / Grok Build 切到 Grok 4.6。  
> 自助充值：[https://littlemagic8.github.io/gptplus/purchase-grok.html](https://littlemagic8.github.io/gptplus/purchase-grok.html)  
> 不会操作微信 **aicygg888**（备注：Grok代充）

---

### 复现这些例子的 7 个手法

下面这些是实测帖和官方文档里反复出现的用法，比「把它当 ChatGPT 用」强很多。

#### 1. 短指令 + 一句验收标准，比超长 Prompt 更稳

4.6 的「审美」已经够好。你知道细节就写细；不知道细节，宁可写短，再补一句验收。

高杠杆句式（直接复制）：

```
先按你的判断做出第一版。
做完后打开页面，按真实用户路径点一遍：
1）核心流程能走通
2）空状态 / 错误状态看一眼
3）把你点到的问题和修复列出来
没验证过的，不要写「已完成」。
```

Eric 拿电子表格 App 做过对照：两页详细规格 vs 三句话需求，成品几乎一样；真正拉开差距的就是上面这句「自己点开验一遍」。

#### 2. 先定义「什么叫做完」，别让模型自己宣布完工

4.6 会自己往下干很久，不需要你喊「继续努力」。它缺的是停损线。

```
完成标准：
- 本地能跑起来
- 主路径截一张图给我
- 列出你改过的文件和没做的部分
- 不要在总结里说 done，除非你已经实际运行过
```

3D、视频、物理这类「看一眼截图验不了」的活，要明确验收方式：录几帧、列问题、只修这些问题。空喊「把贴图做得更好」基本无效。

#### 3. 用同步小步，而不是一次甩大包

4.6 又快又密，适合：

1. 先要一个能跑的骨架
2. 看 30 秒
3. 改一处最刺眼的
4. 再进入下一轮

异步甩一夜当然也能做，但你第二天要冷启动 review 一份大 diff。在乎成品时，4.6 更适合坐在旁边一起做。

#### 4. 视觉 / 交互项目，让它先给「完整第一版」

官方和实测都指向同一点：4.6 第一次就会把结构、配色、交互立住。别一上来就把需求拆成 20 个微任务。

更好的开场：

```
做一个给新用户 10 秒能看懂的 [产品]。
先定信息架构和视觉语言，再实现主路径。
参考：[竞品 / 截图 / 链接]
不要先写文档，直接出能点的版本。
```

#### 5. 知识工作：强制出处和时效

Grok 能搜网页和 X，但你不写清楚，它偶尔会用训练记忆充数。

```
只使用过去 7 天的公开来源。
每条结论后面跟链接。
分三块写：事实 / 推断 / 我还不确定的。
如果搜不到，就说搜不到，不要编。
```

#### 6. 写代码时，把浏览器 QA 编进任务

4.6 能自己点网页、自己申请 API Key、自己做功能 / 视觉 QA。这是它相对很多模型的优势。

```
改完后：
1. 启动本地预览
2. 用浏览器走一遍注册 → 创建 → 保存 → 刷新
3. 截图 + 说明哪里坏了
4. 修完再走一遍，只交能复现通过的结果
```

#### 7. 额度怎么花才不亏

付费档现在是 **每周共享额度池**。聊天便宜，长视频和长编码贵。

- 日常问答、改稿：用 Auto / 普通对话
- 长任务、跨仓库、做产品：再上 4.6 High / Expert
- 生视频是额度黑洞，720p 触顶会自动掉到 480p
- 看消耗：grok.com → **设置 → Usage**，能看到 Chat / Imagine / Voice / Build 各自占比和下次重置时间
- 经常触顶，升级比反复买 Extra Credits 更划算

想把 4.6 放到「关电脑也继续跑」的同事里用，看另一篇：[Grok Bot 上手教程](https://littlemagic8.github.io/2026/08/13/how-to-do-use-grok-bot/)。

---

## 套餐怎么选：SuperGrok 还是 Heavy

以 2026 年 8 月官网公开信息为准。Heavy 的标价不在价格页主卡片上印死，社区和历史档长期按 **约 $300/月** 在谈，偶有促销到 $99 过渡期。下单前以 grok.com 结算页为准。

| 档位 | 大概价格 | Grok 4.6 | Imagine 图/视频 | Grok Build | Grok Bot | 适合谁 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 免费 | $0 | 很少 / 排队 | 基本没有 | 无 | 无 | 试试聊天 |
| SuperGrok Lite | 约 $10 | 有限 | 很少 | 有限 | 无 | 轻度试用 |
| **SuperGrok** | **$30/月** | **有，日常主力** | 有（720p 视频） | **有** | 无 | 大多数创作者 / 开发者 |
| SuperGrok Plus | $100/月 | 有，额度更高 | **1080p**、更高用量 | 更高 | 无 | 重度生视频 / 怕排队 |
| **SuperGrok Heavy** | **约 $300/月** | 最高优先 | 最高档 | 最高档 + 新功能先吃 | **有** | 要 Grok Bot、要先用新功能 |
| Cursor Ultra | $200/月 | 有 | 走 Cursor 体系 | 有 | **有** | 已经在 Cursor 里写代码 |
| X Premium+ | 约 $40/月 | X 里能用 Grok | 另一套额度 | 早期也曾给 Build | 无 | 人在 X 上，不专门为 Grok |

选购口诀：

1. **先用模型、生图、写代码** → SuperGrok $30
2. **视频经常 1080p、额度总爆** → SuperGrok Plus $100
3. **要 Grok Bot / 抢先体验新功能** → SuperGrok Heavy（[Bot 怎么装看这篇](https://littlemagic8.github.io/2026/08/13/how-to-do-use-grok-bot/)）
4. **已经付了 Cursor Ultra** → 先打开 Grok Bot，别重复再买一份 Heavy
5. **人在 X，只是顺便用 Grok** → Premium+；专门用 Grok 更建议官网 SuperGrok（更便宜，额度独立）

> SuperGrok 不是绝对无限。现在是每周额度池 + Fair Use。普通使用几乎感觉不到墙，连续猛生视频、开超长 Agent 会软限流。触顶后可以买 Extra Credits、开 Auto Top Up，或直接升档。升档通常比反复加油包更划算。

---

## 国内订阅 SuperGrok / SuperGrok Heavy

官网要国际 Visa / Master。国内最稳的是 **自助代充**：不用给账号密码，只要 **Grok userId + 卡密**，后台升级。SuperGrok $30 和 SuperGrok Heavy $300 都走这条。

### 步骤 1：买对应档位的充值码

打开自助站（浏览器打开）：

**[https://littlemagic8.github.io/gptplus/purchase-grok.html](https://littlemagic8.github.io/gptplus/purchase-grok.html)**

![SuperGrok 自助充值两步](/img/2026-08-13-grok46/11-purchase.png)

- 只要 Grok 4.6 / Imagine / Grok Build → 买 **SuperGrok $30**
- 要 Grok Bot → 买 **SuperGrok Heavy**
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

3. 确认卡密档位对（$30 还是 Heavy），点 **确定并升级**

![绑定账号后确认升级](/img/2026-08-13-grok46/14-recharge-form.png)

4. 等 2～5 分钟
5. 刷新 grok.com，或退出再登录

### 步骤 4：确认到账

打开 **账户 → 设置 → 订阅**，应看到 **SuperGrok** 或 **SuperGrok Heavy**。

![在设置里确认订阅到账](/img/2026-08-13-grok46/16-sub-check.png)

没立刻显示时：

- 清缓存 / 无痕再登
- 等几分钟（延迟正常）
- 确认登录的是同一个邮箱
- 还不行就拿 userId 和订单找客服

到账后：

- **SuperGrok**：grok.com 切 Grok 4.6，Cursor / Grok Build 里也能用
- **SuperGrok Heavy**：再去 [cursor.com/bot/onboarding](https://cursor.com/bot/onboarding) 下载 Grok Bot，用同一套 Cursor / xAI 登录。安装步骤见 [Grok Bot 教程](https://littlemagic8.github.io/2026/08/13/how-to-do-use-grok-bot/)。

### 官网自己绑卡（有外卡的人）

1. 登录 grok.com
2. 打开 [https://grok.com/supergrok](https://grok.com/supergrok) 或 [价格页](https://x.ai/pricing)
3. 选 SuperGrok / Plus / Heavy
4. 账单之后在 [https://grok.com/?_s=billing](https://grok.com/?_s=billing) 管理
5. 广告拦截有时会挡住「管理订阅」，换无痕窗口

X Premium+ 和 grok.com 订阅是两套账。只为 Grok，优先官网。

---

## 常见问题 FAQ

**Q1：只用 Grok 4.6，必须买 Heavy 吗？**  
不必。SuperGrok $30 就能在 grok.com、Cursor、Grok Build 用 4.6。Heavy 的关键增量是 **Grok Bot + 最高额度 + 新功能先吃**。

**Q2：Grok Bot 和 grok.com 聊天、Grok Build 是一回事吗？**  
不是。grok.com 是聊天 / 生图；Grok Build 是终端写代码；Grok Bot 是云电脑上的常驻同事。Grok Bot 的安装和用法单独写在 [这篇](https://littlemagic8.github.io/2026/08/13/how-to-do-use-grok-bot/)。

**Q3：Grok 4.6 比 Claude / GPT 强在哪？**  
综合智力和 Sol 一档，比 4.5 明显能打长任务。优势是 **又快又便宜、第一版产品完整、会自己点网页验收**。硬核仓库题、终端压测上，Sol / Fable 仍可能更稳。当默认主力很合适，别指望单项世界第一。

**Q4：国内网络怎么访问？**  
需要稳定线路，尽量固定节点，别今天美西明天日本。grok.com 和 X 两套账号可同时用，额度独立。

**Q5：额度用完怎么办？**  
设置 → Usage 看剩余和重置时间。可以买 Extra Credits（目前主要在网页）、开 Auto Top Up，或升 Plus / Heavy。经常触顶就升档，比加油包便宜。

**Q6：代充安全吗？要不要密码？**  
正规代充只要 userId，不要密码、不要验证码。本站跑了很久，SuperGrok / Heavy 都支持。入口：[purchase-grok.html](https://littlemagic8.github.io/gptplus/purchase-grok.html)

**Q7：已经有 Cursor Ultra，还要 Heavy 吗？**  
先打开 Grok Bot。Ultra 已包含 Bot。只有还要 grok.com 上最高档 Imagine / 优先队列时，才考虑再叠 Heavy。

**Q8：订阅后 App 里看不到？**  
确认桌面 / iOS / 网页登录的是同一个 Apple / Google / 邮箱账号。Hide My Email 这类中转邮箱很容易登错号。先退出、清缓存、无痕再登。

---

## 总结：现在最合理的玩法

| 你的目标 | 现在就做 |
| :--- | :--- |
| 体验 Grok 4.6 | 订 SuperGrok，去 Cursor / Grok Build 吃首周 2 倍额度 |
| 出图、出视频、写长文 | SuperGrok；视频很重再看 Plus |
| 把想法做成能点的第一版 | 4.6 + 短需求 + 「自己点开验收」 |
| 养 24 小时 AI 同事 | SuperGrok Heavy 或 Cursor Ultra，看 [Grok Bot 教程](https://littlemagic8.github.io/2026/08/13/how-to-do-use-grok-bot/) |
| 国内付款 | [自助代充](https://littlemagic8.github.io/gptplus/purchase-grok.html) 或微信 aicygg888 |

**一句话：**  
Grok 4.6 是现在性价比最高的前线模型之一，适合当日常默认引擎。大多数人先上 SuperGrok 吃模型，真正有重复流程再上 Heavy 玩 [Grok Bot](https://littlemagic8.github.io/2026/08/13/how-to-do-use-grok-bot/)。

---

## 联系我们

充值、选型卡住，直接找我们。

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
> - [Grok Bot 怎么用 / SuperGrok Heavy](https://littlemagic8.github.io/2026/08/13/how-to-do-use-grok-bot/)
> - [国内订阅 SuperGrok](https://littlemagic8.github.io/2026/04/08/how-to-use-supergrok/)
> - [Grok Build 安装与使用](https://littlemagic8.github.io/2026/06/24/how-to-use-grok-build/)
> - [X Premium+ 订阅](https://littlemagic8.github.io/2026/08/02/how-to-use-X-premium+/)
