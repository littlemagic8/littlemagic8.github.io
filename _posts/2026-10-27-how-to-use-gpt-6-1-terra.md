---
layout:     post
title:      GPT-6.1 Terra 发布了 Terra是什么、谁能用？怎么样？官网测评和真实场景，附 GPT Plus/Pro 国内代充
subtitle:   GPT-6.1 Terra主打电脑操作和自然写作，价格实惠
date:       2026-10-27
author:     aicygg888
header-img: img/post-bg-cook.jpg
catalog: true
tags:
    - GPT-6
    - GPT-6.1 Terra
    - ChatGPT
    - ChatGPTPlus代充
---

10 月 27 日凌晨 2 点刚过，OpenAI 发布了 **GPT-6.1 Terra**。**GPT-6.1 Terra** 主打两件事：看屏幕、操作电脑，以及写作——写得更清楚、更自然。标准 API 价格比 GPT-5.6 Terra 和 GPT-6.1 Sol 低 50%。

![OpenAI 发布图：Introducing GPT-6.1 Terra](/img/2026-10-27-how-to-use-gpt-6-1-terra/01-announce.jpg)

本文主要包含：

1. **GPT-6.1 Terra 是什么**
2. **哪些用户能用**，需要订阅的用充值系统：[https://littlemagic8.github.io/gptplus/purchase-gpt.html](https://littlemagic8.github.io/gptplus/purchase-gpt.html)（浏览器打开）
3. **能做什么，什么场景用？什么时候选择 Sol 或 Astra**
4. **官网测评展示**
5. **网上的真实场景和第三方测评**
6. **价格和调用时要看的几条**

> ps：Terra 只有 Plus 会员以上的用户可以用。需要订阅 GPT Plus 的童鞋，可以使用充值系统：[https://littlemagic8.github.io/gptplus/purchase-gpt.html](https://littlemagic8.github.io/gptplus/purchase-gpt.html)（浏览器打开）

---

## 一、GPT-6.1 Terra 是什么？

官网是这样说的：一个又快、又省的模型，把微小的视觉理解和准确的电脑操作放在一起，写作也更清楚、更自然。相对 GPT-5.6 Terra，这是一次明显的升级。

它适用的是工作日里那些又碎又多的活：写方案、看工程图、填表、剪视频。最常见的例子是把发票读进会计软件。

OpenAI 这些模型可以按用途汇总如下：

| 模型 | 用途 |
|------|------|
| GPT-6 Luna | 轻量、大量任务 |
| GPT-6.1 Terra | 看图、操作电脑、日常写作 |
| GPT-6.1 Sol | 接近 Astra 的复杂工作 |
| GPT-6 Astra | 能力上限 |

API 模型名是 **`gpt-6.1-terra`**。输入是文字和图片，输出是文字。上下文 105 万 token，单次最多输入 92.2 万、最多输出 12.8 万。知识截止日期是 **2026 年 6 月 1 日**。GPT-6.1 Sol 的截止日期是 2026 年 4 月 30 日。

推理强度从 `none`、`low`、`medium`、`high`、`xhigh` 到 `max`，默认是 `medium`。工具调用走 **Responses API**。Chat Completions 也能调这个模型，网页搜索、电脑操作、代码解释器这些工具挂在 Responses 上。不支持微调，也不直接收发音频或视频。

---

## 二、哪些用户能使用 GPT-6.1 Terra？

Plus、Pro、Business、Enterprise、Edu 在 ChatGPT Work 和 Codex 里用，模型列表里选 **GPT-6.1 Terra**。这不是「只有 Free 没有」。Plus 及以上打开 ChatGPT 直接对话，也没有 Terra，要进 ChatGPT Work 或 Codex。Free 先开通 Plus，开通后同样去这两个地方用。开发者走 API，模型名 `gpt-6.1-terra`。

| 在哪里用 | 谁能用 |
|----------|--------|
| ChatGPT Work | Plus、Pro、Business、Enterprise、Edu |
| Codex | Plus、Pro、Business、Enterprise、Edu |
| ChatGPT 直接对话（Plus 也没有） | 没有 Terra |
| OpenAI API | 开发者，模型名 `gpt-6.1-terra` |
| GitHub Copilot | Copilot 应用、CLI、VS Code 已可用 |

GitHub 早期测试里，Terra 完成的终端任务和 C# 编程任务明显多于 GPT-5.6 Terra。范围清楚的任务会收成更集中的几步。日常 agent 编程和终端工作的成本低于 GPT-6.1 Sol。

### 用量额度

同样的用量额度，Terra 能完成的任务比 GPT-5.6 Terra 多，也比 GPT-6.1 Sol、GPT-6 Astra 多。账号里实际还能跑多少，看用量条。

> ps：OpenAI 内部人员 Tibo 这么说：Terra 的用量是 6.1 Sol 的 2 倍，API 和订阅都算，也兑现了上周说的「本周有发布」。他还说，这是他们第一个在写作、个性和理解要求上明显更强的模型，电脑操作也很好。

---

## 三、国内怎么开通：GPT Plus 代充

想要使用 GPT-6.1 Terra，必须是 **Plus** 以上会员（Enterprise、Edu 也可以）。需要订阅 GPT Plus 的童鞋，可以使用充值系统：[https://littlemagic8.github.io/gptplus/purchase-gpt.html](https://littlemagic8.github.io/gptplus/purchase-gpt.html)（浏览器打开）

1. 打开上面的充值系统，支付宝或微信付款。
2. 页面发货卡密。一般几分钟到账，按页面提示操作，不需要把密码发给客服。
3. 到账后刷新 ChatGPT。头像或设置里出现 Plus，再在 ChatGPT Work 或 Codex 里使用 Terra。

已经是 Plus、Pro、Business、Enterprise 或 Edu 的，在 ChatGPT Work 和 Codex 的模型列表里选 GPT-6.1 Terra。充值系统开通的是 Plus。限额仍按官网套餐。

> 充值遇到问题，微信 **aicygg888**，备注 **GPT代充**。

### 常见问题

**充到哪里？**
充进你自己的 ChatGPT 官网账号。不用把密码发给客服。

**Free 充完就能用 Terra 吗？**
充值系统开通的是 Plus。开通后在 ChatGPT Work 和 Codex 的模型列表里选 GPT-6.1 Terra。限额仍按官网套餐。

**已经是 Plus，还要再充一次吗？**
不用。在 ChatGPT Work 和 Codex 的模型列表里选 GPT-6.1 Terra。

**Enterprise、Edu 呢？**
这两档也可以用 Terra。充值系统开通的是 Plus。

**多久到账？**
一般几分钟。超过充值页写的时间还没有 Plus，把订单号发给 aicygg888，备注 **GPT代充**。

---

## 四、能做什么，什么场景用？什么时候选择 Sol 或 Astra

### 电脑操作

Agents’ Last Exam 测的是用软件做专业任务。例子：把建筑图做成 3D 模型，把一部动画逐镜头做成带时间码的修复日志。

- 中等推理：比 GPT-5.6 Terra 高 **15 个百分点**，成本大约是它的 **三分之一**。
- 和 GPT-6 Astra 的成绩打平，每 token 价格大约是 Astra 的 **十分之一**。
- 最高推理：token 效率是 Claude Opus 5.5 的 **3 倍以上**，每 token 价格是它的 **四分之一**，单任务成本大约低到 **九分之一**。
- 完成任务的速度比 GPT-6 Astra 和 GPT-6.1 Sol 都快 **3 倍以上**。

OSWorld 2.1 测的是在桌面软件里做多步操作，例子同样是按工程图做 3D 模型。中等推理下，Terra 超过了 GPT-5.6 Terra 的最好成绩，单任务成本只是后者的一个零头。

发布当天已有人拿它剪视频、做 3D。

### 看图能力

MMMU-Pro 测视觉推理。每个推理档位都超过 GPT-5.6 Terra，成本低很多的时候接近 GPT-6 Astra 和 GPT-6.1 Sol。

### 少犯错

一组容易诱发错误的内部题目上，低推理强度的错误率从 GPT-5.6 Terra 的 **53.6%** 降到 Terra 的 **16.7%**。最高强度下再降到 **4.3%**，接近 Astra 和 Sol。

### 代码能力

Terminal-Bench 4.0 测的是在命令行里修问题。例子：页面一边加载一边跳动，把这个布局问题修好。最高推理下，Terra 解出 **50.3%**，GPT-5.6 Terra 已公布的成绩是 **21.5%**。

Terminal-Bench-Science 0.1 测的是用代码做科研步骤，例子是在延时视频里跟踪细胞分裂。最高推理下，Terra 以更低的成本超过 GPT-6.1 Sol，和 Opus 5.5 的差距在 5 分以内，估算成本不到它的五分之一。

最复杂的编程，用 **GPT-6.1 Sol** 或 **GPT-6 Astra**。这两档在复杂编程上通常更稳。

### 安全

按 Preparedness Framework，Terra 的网络安全能力达到 Critical 这一档，并沿用了 GPT-6 Astra 的防护。和 GPT-5.6 Terra 比，它更常守住任务范围，也会把做不到的地方说出来。提示注入测试里，它对把模型拽离用户任务的指令抵抗较强。

### 怎么选

| 你要做的事 | 更合适的选择 |
|------------|----------------|
| 看屏幕、填表、录发票、看工程图、剪视频、日常写作 | GPT-6.1 Terra |
| 浏览器里的多步操作 | Terra。Browser Use 的榜上，high 档 78.5，Sol 是 79.7 |
| 命令行里范围清楚的修改、终端活 | Terra。完成的终端和 C# 任务多于 5.6 Terra，成本低于 Sol |
| 数据分析，要快、要便宜 | Terra。Plotly 的卷子是 40/43。要满分用 Sol |
| 会计分类、分录，成本敏感 | Terra 这两项高。结账、应收应付要逐次核对 |
| 最复杂的编程、深入研究 | **GPT-6.1 Sol** 或 **GPT-6 Astra** |
| 修 bug，且推理不是 max | 先别用 Terra 的 xhigh、high。Huryn 的 105 个 bug 里，这两档掉得很快，要那个成绩对应的是 max |

写方案、改语气，直接用 Terra。

---

## 五、官网测评展示

### Agents’ Last Exam

浅绿是 GPT-6.1 Terra，深绿是 GPT-5.6 Terra，青色星是 GPT-6.1 Sol，蓝色星是 GPT-6 Astra，灰色菱形是 Claude Opus 5.5。横轴是成本，纵轴是分数。Terra 的一串点在左侧，Astra 和 Opus 5.5 在更贵的右侧。

![OpenAI：Agents’ Last Exam v1，分数和成本](/img/2026-10-27-how-to-use-gpt-6-1-terra/02-agents-last-exam.png)

### Terminal-Bench 4.0

浅绿 GPT-6.1 Terra 的高点在 50% 附近，对应 50.3%。深绿 GPT-5.6 Terra 在 20% 出头，对应 21.5%。Sol 的曲线在 Terra 上方一点，Claude Sonnet 5.5 的高点更靠右，也更高。

![OpenAI：Terminal-Bench 4.0，分数和成本](/img/2026-10-27-how-to-use-gpt-6-1-terra/05-terminal.jpg)

---

## 六、社区的真实场景和第三方测评

### 1. 适用的工作

- 写方案、改写、把话说顺
- 看工程图、建筑图，做成 3D
- 填表，把发票录入会计软件
- 剪视频，逐镜头做时间码日志
- 修加载时乱跳的网页
- 在延时视频里跟踪细胞分裂

### 2. Plotly：数据分析 40/43，整卷 1.31 美元

Plotly 在发布当天用 DataAnalyticsBench 跑了一遍。考卷不公开，数据是虚构的风电场。Terra 用的是默认推理。

| 模型 | 得分 | 整卷费用 | 每题中位时间 |
|------|------|----------|----------------|
| GPT-6 Luna | 38/43 | 0.13 美元 | 18 秒 |
| GPT-6.1 Terra | 40/43 | 1.31 美元 | 15 秒 |
| GPT-6.1 Sol | 43/43 | 2.61 美元 | 18 秒 |

他们测过的 35 个模型里，拿到 40 分及以上的模型中，Terra 最快。常规分析、含糊题、做不到的请求、数据质量题都满分。丢的 3 分在更难的地方：5 个埋进数据里的规律找出了 3 个，还有一道亚北极产能的题没有追到原因。大约每题 15 秒、输出约 1460 token、每题大约 4.5 次调用。

### 3. DualEntry：记账很快、很便宜，准确率不是第一

101 道会计题，Terra **78.2%**，22 个模型里并列第 18。GPT-6.1 Sol 和 GPT-6 Astra 都是 81.2%，Gemini 4 Argon 是 91.1%。它排在 Claude Haiku 5.5、GPT-6 Sol（都是 76.2%）和 GPT-6 Luna（66.3%）前面。

交易分类 13/13，会计分录 12/13，银行对账 10/12。应付、应收和月结关闭落到 53.8% 到 58.3%。简单题 37 道对了 28 道。三次都做对的任务占 65.3%。

平均每题 16.1 秒，第三快（Haiku 5.5 是 11.4 秒，Sonnet 5.5 是 12.1 秒）。Sol 是 27.2 秒，Astra 是 34.3 秒。每题约 0.042 美元，大约是 Astra 的十分之一、Sol 的一半。

分类、分录这种结构清楚的活，Terra 合适。结账要每次都对，榜上更稳的模型排在前面。

### 4. Browser Use：浏览器操作接近 Sol

Browser Use Benchmark v2.1，160 道共用题，16 个模型。**GPT-6.1 Terra high 是 78.5**，**GPT-6.1 Sol high 是 79.7**，成本低 35%。档位是 high。

![Browser Use Benchmark v2.1：Terra high 78.5，Sol high 79.7](/img/2026-10-27-how-to-use-gpt-6-1-terra/06-browser-use.jpg)

### 5. 修 bug：max 档有效，再低一档掉得很快

Paweł Huryn 用 2 个仓库、105 个重新种下的 bug，让模型自己找、自己改。只计算种下的 bug。Codex CLI，3 次运行：

| 模型 / 档位 | 种下的 bug | 耗时 | 费用 |
|-------------|------------|------|------|
| GPT-6.1 Terra max | 40.7/105 | 37.3 分钟 | 3.88 美元 |
| GPT-5.6 Terra max | 32/105 | 159.7 分钟 | 27.98 美元 |
| GPT-6.1 Terra xhigh | 11.3/105 | 15.9 分钟 | 0.75 美元 |
| GPT-6.1 Terra high | 9.7/105 | 12.6 分钟 | 0.56 美元 |

同一次测试里，GPT-6.1 Sol max 是 44.3/105、5.88 美元，GPT-6 Astra max 是 45/105、33.03 美元。Haiku 5.5 的 xhigh 是 18.3/105。max 档又快又便宜；离开 max，成绩掉到 Haiku 5.5 xhigh 下面。

![Bug Hunt Bench：GPT-6.1 Terra 在 max 为 40.7/105，xhigh 和 high 明显更低](/img/2026-10-27-how-to-use-gpt-6-1-terra/07-pawel-bugs.jpg)

### 6. Artificial Analysis：更聪明，单任务更便宜，乱猜变少

Intelligence Index 上，**GPT-6.1 Terra（max）是 48**，**GPT-5.6 Terra（max）是 42**，**GPT-6.1 Sol（max）是 52**。max 档比 5.6 Terra 高 6 分，单任务成本从 1.40 美元降到 **0.40 美元**，比 Sol 低 4 分。低档和中档落在成本效率前沿上。

另外三组成绩：

- **AA-Omniscience**：不知道答案时还在猜的比例，从 5.6 Terra 的 88% 降到 38%，准确率同时高 2 分。这和前面的 16.7% 错误率不是同一套题。
- **Coding Agent Index v2.0**：Terra 48，Sol 54，Luna 31。
- **Terminal-Bench 4.0**：大约加 20 分，max 档接近 Sol。

价格核对：Terra 是每百万 token 输入 1 美元、输出 5 美元；5.6 Terra 是 2 美元和 12 美元。缓存命中从 0.20 美元降到 0.05 美元。

![Artificial Analysis Intelligence Index：Terra max 为 48，5.6 Terra max 为 42，Sol max 为 52](/img/2026-10-27-how-to-use-gpt-6-1-terra/04-aa-index.jpg)

---

## 七、价格和调用时要看的几条

标准价，每百万 token：

| 项目 | 价格 |
|------|------|
| 输入 | 1 美元 |
| 缓存输入 | 0.05 美元 |
| 输出 | 5 美元 |

另外几条计费规则：

> 命中缓存的读取是 0.05 美元。把内容写进缓存另算：保留 30 分钟是每百万 token 1.25 美元，保留 12 小时是 2.50 美元。
>
> 输入超过 27.2 万 token 的请求，输入和缓存按 2 倍、输出按 1.5 倍，整次请求都按这个倍率。
>
> Batch 和 Flex 是标准价的 50%。Fast 模式是标准价的 2 倍。部分地区处理加 10%。工具按次另有费用。

调用时记这三条：

1. 模型名写 **`gpt-6.1-terra`**。
2. 要用电脑操作、网页搜索、代码解释器、文件搜索、MCP，走 **Responses API**。
3. 默认推理是 `medium`。50.3%、高 15 分这些数字都带档位。Huryn 的修 bug 测试里，max 和再低一档差得特别大。

---

## 最后

- GPT-6.1 Terra 面向看图、操作电脑和日常写作，比 GPT-5.6 Terra 便宜，低推理时也更少说错。
- Plus、Pro、Enterprise、Edu 可在 ChatGPT Work 和 Codex 里用，API 名是 `gpt-6.1-terra`。GitHub Copilot 也已加上。
- 电脑操作上，中等推理打平 Astra，每 token 大约十分之一的价格，速度是 Astra 和 Sol 的 3 倍以上。
- 命令行编程从 21.5% 到 50.3%。最复杂的编程用 Sol 或 Astra。
- 公开测评里它通常又快又便宜：Plotly 40/43，Browser Use 78.5 对 Sol 的 79.7。会计准确率，以及把推理调离 max 之后的修 bug，没有一起站上第一。

需要订阅 GPT Plus 的童鞋，可以使用充值系统：[https://littlemagic8.github.io/gptplus/purchase-gpt.html](https://littlemagic8.github.io/gptplus/purchase-gpt.html)（浏览器打开）

## 参考资料

- [OpenAI：Introducing GPT-6.1 Terra](https://openai.com/index/introducing-gpt-6-1-terra/)
- [OpenAI Help：GPT-6.1 Terra 不在 Chat，在 Work 和 Codex](https://help.openai.com/en/articles/20001354-gpt-6-and-other-models-in-chatgpt)
- [OpenAI 发布帖](https://x.com/OpenAI/status/2114780711664398349)
- [模型页 gpt-6.1-terra](https://developers.openai.com/api/docs/models/gpt-6.1-terra)
- [API 价格页](https://developers.openai.com/api/docs/pricing)
- [系统卡附录](https://deploymentsafety.openai.com/gpt-6-1-terra)
- [Tibo，Day 22](https://x.com/thsottiaux/status/2114800277677092936)
- [Victor E. Nunez](https://x.com/victornunez/status/2114781066892378396)
- [Artificial Analysis](https://x.com/ArtificialAnlys/status/2114781865811063259)
- [Plotly DataAnalyticsBench](https://plotly.com/blog/gpt-6-1-terra-plotly-data-analytics-bench/)
- [DualEntry 会计测评](https://www.dualentry.com/blog/gpt-6-1-terra-accounting-benchmark)
- [Browser Use](https://x.com/browser_use/status/2114901176575725623)
- [Paweł Huryn / Bug Hunt](https://x.com/PawelHuryn/status/2114860186330398962)
- [GitHub Copilot](https://x.com/github/status/2114799272634007801)

## 联系我们

充值过程中遇到任何问题，或有其他业务需求，请联系我们。

请保存网址 [https://littlemagic8.github.io/gptplus/](https://littlemagic8.github.io/gptplus/) ，并加上联系方式，防止失联。

防失联客服微信：

```
aicygg888
```

添加好友请备注：**GPT代充**（加的人多，微信防频繁，请扫码）

## 小提示：想用更多 AI 产品，可以联系 V: aicygg888

> **如果不想开通信用卡，可参考：无需开通信用卡完成 ChatGPT 订阅教程。**
>
> ChatGPTplus 独享账号升级充值自助平台：[https://littlemagic8.github.io/gptplus/](https://littlemagic8.github.io/gptplus/)（网站下方有购买卡密和使用教程）
>
> GPT 代充直达：[https://littlemagic8.github.io/gptplus/purchase-gpt.html](https://littlemagic8.github.io/gptplus/purchase-gpt.html)（支付宝/微信付款，几分钟到账，无需账密）
>
> 开通自己的 ChatGPT Plus、Claude Pro 个人独享账号，可参考：[使用支付方式订阅开通 ChatGPT Plus、Claude Pro 教程](https://littlemagic8.github.io/2024/09/04/update-ChatGPT-Plus/)
>
> **国内使用 ChatGPT / Claude 镜像账号，有两种方式：**

**方式一：官网镜像（chatgpt官网共享账号，国内网络可访问）按教程自行购买**

遇到问题联系微信：aicygg888

登录地址：https://chatshare.biz/ （复制到浏览器打开，用购买成功后的账号密码登录）
购买地址：https://littlemagic8.github.io/buychat/

- [ChatGPT Plus 独享账号教程](https://littlemagic8.github.io/2025/07/17/chatgptplus-auto-system/)
- [Claude Pro 订阅指南](https://littlemagic8.github.io/2024/12/09/ChatGPT-and-Cluade/)
- [镜像账号使用说明](https://littlemagic8.github.io/2025/07/17/chatgptplus-chatshare/)

**方式二：不想自己注册，添加微信购买**

微信：**aicygg888**（备注：镜像账号）

欢迎加微信：

![微信客服](/img/2026-08-02-x-premium-plus/wechat-qr.png)

公众号也可以哦：

![公众号](/img/v2-4e622b64238b20948a02e0c988ca5704_720w.png)
