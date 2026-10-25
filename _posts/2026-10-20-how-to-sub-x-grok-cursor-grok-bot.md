---
layout:     post
title:      X、Grok、Cursor、Grok Bot 四合一订阅教程(附自助充值流程)：开通与取消自动续费
subtitle:   一个套餐管理 X、Grok、Cursor 和 Grok Bot；Premium 及以上的 Grok Bot 会把任务路由到 Claude Opus 5.5，附官网订阅、账单及取消续费步骤
date:       2026-10-20
author:     aicygg888
header-img: img/post-bg-cook.jpg
catalog: true
tags:
    - XSubscription
    - X
    - Grok
    - Cursor
    - GrokBot
---

X、Grok、Cursor 和 Grok Bot 现在可以通过 **The X Subscription** 统一管理：一个工作区、一份账单和一个套餐。本文介绍如何选择档位、在网页上完成订阅，以及订阅成功后如何关闭自动续费。

> 本文以网页版直接订阅为例。页面名称、可选套餐和价格会随地区或活动变化，请以结账页显示为准。

## 一、四合一订阅是什么？

The X Subscription 将以下能力放在同一个套餐中：

| 产品 | 订阅后如何使用 |
| --- | --- |
| **X** | 绑定个人 X 账号后获得与所选档位对应的 X 权益 |
| **Grok** | 使用套餐包含的 Grok 模型和额度 |
| **Cursor** | 在同一工作区中使用 Cursor；Grok 和 Cursor 共用套餐的周度额度 |
| **Grok Bot** | Premium、Super、Ultra 包含。系统会按任务把后端切到最合适的模型，官方点名说含有 Claude Opus 5.5 |

需要注意的是，**Grok Bot 不包含在 Plus 档位内**。如果目标是 X、Grok、Cursor、Grok Bot 四合一，并且希望难的任务可以走到 Claude Opus 5.5，请选择 **Premium 或更高档位**。在 Cursor 编辑器里自己点选 Claude 或 GPT，不属于套餐的共享额度，可能会从额外预付额度中计费。Grok Bot 自动路由到 Opus 5.5 是另一条路径，见第三节。

官方将 Grok、Cursor 和 X 整合在一个套餐中；Grok、Cursor 与 Grok Bot 共用对应档位的周度用量池。[查看 The X Subscription 官方说明](https://docs.x.ai/x-subscription/overview) · [查看 Grok Bot 套餐说明](https://docs.x.ai/x-subscription/grok-bot)

## 二、套餐怎么选？

当前个人套餐的官方标价如下，实际税费和活动折扣以结账页为准：

| 档位 | 月付标价 | 适合场景 | Grok Bot |
| --- | ---: | --- | --- |
| Plus | $8 / 月 | 主要使用 X 和基础 AI 权益 | 不包含 |
| Premium | $30 / 月 | 需要四合一能力的个人用户 | 包含 |
| Super | $100 / 月 | 高频使用 Grok、Cursor 或 Grok Bot | 包含，额度更高 |
| Ultra | $200 / 月 | 对用量和优先级要求更高的用户 | 包含，额度最高 |

官方说明中，Premium、Super、Ultra 的包含用量分别约为 Plus 的 4 倍、15 倍、50 倍。截图中的折扣或金额可能是特定活动展示，**不要将截图中的促销价格当作固定价格**。[查看官方套餐与价格](https://docs.x.ai/x-subscription/pricing)

![选择 The X Subscription 套餐档位](/img/2026-10-20-x-subscription-guide/plan-selection.png)

## 三、Grok Bot 会把任务交给 Claude Opus 5.5

2026-10-25 对照了 Cursor 帮助中心的 [Which AI models power Grok Bot?](https://cursor.com/help/grok-bot/models)。Grok Bot 不绑死在一个模型上。每一项任务，它用当时最可能把结果做好的后端：可以是 xAI 自己的模型，也可以是子处理商名单上的第三方模型。帮助中心把 **Claude Opus 5.5** 写进了计费说明。

路由到 Opus 5.5 **不会按 token 另加价**。原文是：routing a task to Opus 5.5 doesn't change what it costs you per token。用得快还是慢，看任务本身有多费劲，用量仍算在套餐的周度共享池里，账单记成 Grok Bot，不按模型拆开。

![Grok Bot 官方说明：路由到 Opus 5.5 不改变每个 token 的价格](/img/2026-10-20-x-subscription-guide/grok-bot-opus.png)

这件事只落在带 Grok Bot 的档位上，也就是 **Premium、Super、Ultra**。Plus 没有 Grok Bot，也就没有这条路由。三个档位的差别是周度额度：官方写的大约是 Plus 用量的 4 倍、15 倍、50 倍。想让难任务有机会走到 Opus 5.5，至少从 Premium 订起。

同一天能核对到的范围就这些：

| 项目 | 官方怎么写 |
| --- | --- |
| 点名的 Claude 模型 | **Claude Opus 5.5**。帮助页没有写 Sonnet、Haiku 或 Fable |
| 谁来选模型 | 系统选。没有模型菜单，不能指定用 Claude，也不能把 Claude 关掉 |
| 能不能看到这轮用了谁 | 不能。用量页只显示 Grok Bot，不显示供应商或模型名 |
| 会不会更贵 | 路由到 Opus 5.5 不改变每个 token 的价格 |
| 谁能用上 | Premium、Super、Ultra。Plus 不含 Grok Bot |
| 模型提供方 | [子处理商名单](https://trust.cursor.com/subprocessors) 里有 Anthropic，身份是推理服务商。名单会变，以页面当时的列表为准 |

10 月 7 日，Elon Musk 也就 Grok Bot 发过一条说明：往后 SpaceX 会为每项任务使用最合适的后端，点名包括 Claude Opus 5.5、MidJourney、Suno 以及其他领先 API，标准是「最可能给你最好的结果」。[原帖](https://x.com/elonmusk/status/2107724314451878104)。帮助中心目前写死的模型名是 Opus 5.5；MidJourney 和 Suno 以这条公开说明为准，产品页没有再单独列出。

> 两套 Claude 不要混在一起。Grok Bot 是系统自动路由，走到 Opus 5.5 不加价。Cursor 编辑器里如果自己选 Claude 或 GPT，仍可能从额外预付额度扣费，见文末关于额外费用的说明。

## 四、订阅前先确认账号

如果你已经订阅了 Cursor、SuperGrok 或 X Premium，可以先将符合条件的个人账号统一到 The X Subscription。这个过程会将选择的账号合并到一个工作区和账单下，完成后**不能撤销**，操作前请确认登录的是正确的个人 X、Grok 和 Cursor 账号。

- 已订阅 Cursor：从 [cursor.com/unify](https://cursor.com/unify) 开始。
- 已订阅 Grok 或 X：从 [accounts.x.ai/unify](https://accounts.x.ai/unify) 或 X 内的订阅升级入口开始。
- 没有付费套餐的新用户：可在 [x.ai/pricing](https://x.ai/pricing) 选择套餐。

直接计费的旧 Cursor、Grok 和 X Premium 套餐会在统一时按规则取消，并按剩余周期计算退款；应用商店计费的情况需按官方说明单独确认。[查看统一账号的官方步骤](https://docs.x.ai/x-subscription/unify-accounts)

## 五、网页版订阅步骤

> tips：自助充值新版四合一X sub传送门：https://littlemagic8.github.io/gptplus/purchase-grok.html

### 第一步：打开订阅入口

登录 X，在右侧的 **Subscribe** 卡片中点击订阅入口。不同账号的入口位置可能略有不同，也可以从订阅或升级页面进入。

![在 X 网页版点击订阅入口](/img/2026-10-20-x-subscription-guide/subscribe-entry.png)

### 第二步：选择套餐

选择适合自己的月付或年付档位。想使用 Grok Bot 时，务必选择 **Premium、Super 或 Ultra**，不要选择 Plus。

![选择需要的套餐档位](/img/2026-10-20-x-subscription-guide/plan-selection.png)

### 第三步：填写账单信息和支付方式

按页面要求填写账单信息，选择可用的银行卡、Apple Pay、Google Pay 或其他可见支付方式。提交前，请再次确认套餐、账期、税费和付款账号。

![填写账单信息并选择支付方式](/img/2026-10-20-x-subscription-guide/billing-information.png)

### 第四步：确认订阅

勾选页面要求的条款后，点击 **Subscribe & Pay** 完成付款。订阅默认为自动续费；如果不打算下个周期继续使用，可以在成功后立即按照下文步骤关闭自动续费。

![点击 Subscribe and Pay 完成订阅](/img/2026-10-20-x-subscription-guide/subscribe-and-pay.png)

### 第五步：确认订阅成功

成功后会出现欢迎页。随后可以在已关联的 X、Grok 和 Cursor 账号中检查权益是否生效；账号绑定或权益同步可能需要一些时间。

![X Subscription 订阅成功页面](/img/2026-10-20-x-subscription-guide/subscription-success.png)

## 六、订阅成功后如何取消自动续费？

取消自动续费不会立即取消当前周期的权益，而是停止下一期自动扣款。官方建议至少在续费前 24 小时完成取消；具体状态和到期日以订阅管理页显示为准。

### 第一步：进入设置和隐私

在 X 网页版点击 **More（更多）**，选择 **Settings and privacy（设置和隐私）**。

![从更多菜单进入设置和隐私](/img/2026-10-20-x-subscription-guide/settings-and-privacy.png)

### 第二步：打开 Premium / Subscription 页面

在设置中选择 **Premium**。然后进入订阅管理页面。

![在设置中选择 Premium](/img/2026-10-20-x-subscription-guide/premium-settings.png)

### 第三步：管理订阅

点击 **Manage your subscription（管理你的订阅）**，进入当前套餐、账单和付款方式页面。

![点击管理你的订阅](/img/2026-10-20-x-subscription-guide/manage-subscription.png)

### 第四步：取消套餐

在 **Cancel subscription（取消订阅）** 区域点击 **Cancel plan（取消套餐）**。

![点击取消套餐](/img/2026-10-20-x-subscription-guide/cancel-plan.png)

### 第五步：完成确认

阅读页面提示后，点击 **Cancel Plus / Cancel Premium** 等确认按钮。按钮名称会随套餐变化。

![确认取消订阅](/img/2026-10-20-x-subscription-guide/confirm-cancellation.png)

### 第六步：检查取消状态

返回订阅管理页后，如果显示 **Canceled subscription（已取消订阅）**、**Expiring（即将到期）** 和具体的可用截止日期，说明自动续费已经关闭。页面通常还会提供 **Renew（恢复订阅）** 按钮，代表你可以在到期前重新开启续费。

![查看已取消订阅和到期日期](/img/2026-10-20-x-subscription-guide/cancellation-confirmed.png)

## 七、账单和额外用量要再检查一次

在订阅管理页的 **Invoices（账单）** 区域可以查看付款状态并下载账单。取消套餐只会停止基础套餐的下一期续费；如果你曾在 Grok 控制台开启 **Auto Top-up（自动充值）** 或添加预付额度，也应到 [Grok Dashboard](https://grok.com/dashboard) 单独检查该开关和消费上限。

![在订阅管理页查看和下载账单](/img/2026-10-20-x-subscription-guide/invoice-download.png)

> **重要：**套餐取消与额外用量的自动充值是两项独立设置。Auto Top-up 默认关闭，只有手动开启后才会按阈值扣款。[查看官方额外用量和自动充值说明](https://docs.x.ai/x-subscription/extra-usage)

## 常见问题

### 取消后还能使用多久？

通常可以使用到当前已付款周期结束。以订阅管理页显示的到期日为准。

### 我原来的 X Premium、Grok 或 Cursor 会不会重复收费？

如果旧套餐被纳入统一流程，官方会按规则取消直接计费的旧套餐并处理剩余周期退款。未被纳入统一的账号、应用商店计费或其他单独购买的套餐，需要自行检查并单独处理。

### 我只订到 Plus，为什么没有 Grok Bot？

Grok Bot 不包含在 Plus 内。请在套餐页面升级到 Premium、Super 或 Ultra 后再使用。Claude Opus 5.5 的自动路由也只在这三档的 Grok Bot 里。

### Grok Bot 能不能自己选择 Claude？

不能。官方写明没有模型选择器，也不能指定或屏蔽某一个模型。它按任务自己决定用 xAI 的模型还是第三方模型。帮助中心点名的是 Claude Opus 5.5，路由过去不按 token 加价，用量仍算在周度共享池里。对话和账单里看不到「这轮用的是 Opus」。

### 怎样控制 Cursor 的额外费用？

套餐的共享用量主要覆盖符合条件的第一方 Grok 使用。Cursor 中的第三方模型可能消耗预付额度；可在 Grok Dashboard 设置月度额外用量上限，并确认是否关闭 Auto Top-up。[查看官方消费上限说明](https://docs.x.ai/x-subscription/spending-caps)

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