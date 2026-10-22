---
layout:     post
title:      Claude Duet怎么用？哪些用户能使用？Duet怎么样？Claude Pro / Max 代充订阅和候补Duet手把手教程
subtitle:   Claude Duet 研究预览保姆级说明：主动干活的智能体、美国 Pro/Max 候补、额度规则，以及国内开通 Claude Pro 的代充步骤
date:       2026-10-22
author:     aicygg888
header-img: img/post-bg-cook.jpg
catalog: true
tags:
    - Claude
    - ClaudeDuet
    - ClaudePro代充
    - Opus5.5
---

2026-10-22 claudeai 官宣 **Claude Duet**：一个会主动来找你的智能体 App，目前是研究预览版。

**Claude Duet**发布了的话，截止目前top级大模型厂家的AI 智能体都上线了

Gemini：Spark
Grok：Bot
OpenAI：dots
Anthropic：Claude Duet
Meta：Muse

它会告诉你哪些事需要处理，做完你交代的任务，退出应用云端还能接着干。代你发消息、付款、签字或删除之前，会先把内容拿给你确认。

底层围着 **Claude Opus 5.5** 设计，沿用你 Claude 账号里的记忆、Skills 和已经连上的应用。体验Duet要同时满足三个条件：**Pro 或 Max**、**这个 Claude 账号在美国**、**官方候补名单发来的邀请邮件**。所以即使是 Pro 或 Max 不能直接使用，要先去产品页排队，Anthropic 分批发邮件。Team、Enterprise，以及不在美国的账号，这一阶段还不能用（需要等等）。Duet 本身不再另收费，统一使用套餐里的额度。

> 还没有 Claude Pro 的童鞋，可以先看第六节的国内代充。代充只把 Free 升成 Pro，账号地区保持原样，也不会附带 Duet 邀请。账号不是美国，或者还没收到邀请邮件，现在都无法体验。
>
> Claude Pro 代充入口：https://littlemagic8.github.io/gptplus/purchase-claude.html （浏览器打开）
>
> 需要 Max，或充值遇到问题，联系客服：aicygg888
>
> 如果需要快速使用上可以试试grok bot，体验下来很不错，参考图文教程：https://littlemagic8.github.io/2026/10/18/how-to-use-grok-bot/

![Claude Duet 产品页和 Join the waitlist 表单](/img/2026-10-22-how-to-use-claude-duet/02-waitlist.png)

产品页：[claude.com/product/claude-duet](https://claude.com/product/claude-duet)

官方介绍：[claude.com/resources/articles/claude-duet](https://claude.com/resources/articles/claude-duet)

## **一、Claude Duet 是什么**

官方原话是：Claude Duet is a proactive agent that understands what needs your attention. 它接手大大小小的任务，你不在的时候继续做，碰到要紧的操作就停下来等你点头。面向的是事情多、容易漏的专业人士和小生意老板。

它是一个**单独的 App**，有 iOS、Android，电脑上从 [claude.ai](https://claude.ai) 打开。研究预览阶段它不在主 Claude App 里面，两边以后怎么合，官方说要看早期用户的反馈。

| 对比项 | 普通 Claude | Claude Duet |
| --- | --- | --- |
| 谁先开口 | 你打开对话，它才开始 | 它早上给你简报，做完或需要决定时来找你 |
| 运行位置 | 跟着当前这次对话 | 自己的云端电脑，关掉手机也能接着干 |
| 账号 | Claude 账号 | 同一个账号，记忆、Skills、Connectors 直接带过来 |
| 模型 | 可以自己选 | 研究预览里不能选，固定 Opus 5.5 |
| 适合 | 问答、写作、写代码、一起改一版稿 | 盯邮件和日历、起草待你确认的回复、把一整件工作做完 |

Opus 5.5 本身的能力和价格，写在之前这篇里：[Claude Opus 5.5 怎么样](https://littlemagic8.github.io/2026/09/23/how-to-use-claude-opus-5.5/)。

## **二、Claude Duet 能做什么**

官方把它收成四件事。

### 1. 早上告诉你该看什么

每天早上发一份短简报，从已连接的邮件和日历里挑出最该处理的几件，并且可以先起草回复，等你过目。白天它隔一段时间再看一遍这些应用，只有真的需要你时才发消息。

官方帮助中心写明：它是**按间隔检查**，不会一刻不停地刷。不停地查会把套餐额度烧得很快。两次检查之间新来的急事，它可能要到下一次才看见。

### 2. 你丢一句话，它把活做完

从小事到整件工作都可以。官方举的例子包括：

- 约会议
- 会前给一家公司做简报
- 用几十个工具拼一个仪表盘
- 做财务或销售预测
- 做原型、做网页应用
- 在 Stripe 或 QuickBooks 里找未付款发票，并起草催款信等你批准
- 在 Gusto 里把工时、奖金、报销填好，工资表准备到等你确认
- 起草招聘启事，你改完并批准后再发到 LinkedIn
- 用 DocuSign 把协议准备到签字
- 按 HubSpot 里的客户和交易记录起草跟进邮件
- 在 Canva 里把产品发布做成社媒方案
- 打理 Shopify 店铺（更完整的可视化装修还在「即将推出」）

比较大的成品，比如简报、财务模型、幻灯片、仪表盘，会出现在 **Make** 标签里，你可以打开再改。进行中的任务在 **Tasks** 里，需要你拍板的会标出来。主对话尽量保持干净：做完了，或者要你决定了，它才在主线程里说一声。它可以建议某件事看起来做完了，**点完成的人仍然是你**。

### 3. 退出应用，云端接着干

Duet 有一台带浏览器的云端虚拟机，不虚脱你的电脑或手机实时开着。你用一句话描述任务，它自己决定用哪些应用、分几步做。做完或需要你看的时候，再发通知。

还没有连接器的网站，它用这台云端浏览器去打开。研究预览里你**还不能看着它操作浏览器，也不能接管那台浏览器**。

### 4. 代你动手之前先问你

发消息、付款、在文件上签字、删除东西，它会把即将执行的内容亮出来，等你批准。你一时没点，它先把任务里别的部分做完，稍后再把这个审批拿回来。

用 Stripe 的 Link 或 Shopify 的 Shop Pay 买东西时，也是先跟你确认商品，再由钱包请你批准这笔支出。Link 会用一次性虚拟卡付款，不把你的真实卡号交出去。这两项目前只在 Duet 里连接，不在普通连接器目录里。

![Claude Duet 可接入的应用，官方称超过 6000 个连接器和插件](/img/2026-10-22-how-to-use-claude-duet/03-connectors.png)

帮助中心点名能接着用的连接器包括 Gmail、Google Calendar、Google Drive、Slack、QuickBooks、HubSpot、Docusign、Calendly。Slack 在 Duet 里有使用限制。**Microsoft 365 研究预览阶段还不可用。** 1Password 登录已保存的网站，官方写的是即将支持，而且要你授权。

## **三、Duet 怎么样**

官方把卖点放在「判断力」上：Opus 5.5 是他们觉得第一款够格主动干活的模型，能分清什么要找你、什么可以等、什么必须先问。

官宣视频里，Anthropic Labs 的 Mike Krieger 说他已经在工作和生活里用了几周：让它起草炉边谈话的问题，周末替他盯 Slack，自己先下线；它还告诉他 Neal Stephenson 的新书，并在他开口之后从本地书店下单。

![Mike Krieger 在 Claude Duet 官宣视频里](/img/2026-10-22-how-to-use-claude-duet/01-announce.jpg)

> 视频原帖：[Mike Krieger](https://x.com/mikeyk/status/2112986420231233951)

Claude Code 和 Cowork 的产品负责人 Cat Wu（[@_catwu](https://x.com/_catwu/status/2112988751576330487)）说，这是在回应大家「希望 Claude 主动多分担一些」的反馈。Duet 会先注意到有工作要做，然后在你开口之前动手。

Every 的 Dan Shipper 测了两周，原话是这是「第一个能算专业工具的个人智能体」（the first personal agent I'd call a pro tool）。他补充的使用感受可以分开看：

- 独立 App，iOS、Android 和网页都有，和主 Claude 分开，上手比较干净
- 可以按工作、生活开不同 channel，不是只有一条聊天
- 有待办列表，能看见每件事做到哪一步
- 在 App 里就能写和改文档、幻灯片
- 还不是「首席幕僚」：能看见他电脑上的 Claude 会话，但不能指挥那些会话
- 邮件草稿他认为不如 OpenAI 的 dots
- 语音目前是转写，还不能跟它语音对谈
- 他的结论是手感不错，每天会打开，值得试

官方自己也把短板写在研究预览说明里，这些比宣传语更值得看：

- 可能读错一封邮件或一条线程，也可能把不急的事判成急事
- 个人杂事，比如订票，不如工作场景稳
- 检查是隔一段时间一次，间隔里新到的消息会漏到下一轮
- 后台简报和巡检都算进 Pro / Max 额度，大任务（财务模型、整套幻灯片）更费
- 不能选模型，也不能看着它的浏览器
- 看不到你电脑上的全部项目和本地文件；能读 Claude 里的工作，但不能改那些对话
- 不能打电话，也不能给别人发短信。经你同意后，可以从已连接的邮箱发信
- 有些事你点了同意也不做：交易证券、在账户之间转账、进入别人的账号

和本站写过的另外两个「会自己干活」的产品放在一起看：[OpenAI dots](https://littlemagic8.github.io/2026/10/08/how-to-use-gpt-dots/) 更偏通用的常驻目标，[Grok Bot](https://littlemagic8.github.io/2026/10/18/how-to-use-grok-bot/) 更偏云电脑上的执行队友。Duet 这一版明显往「工作简报 + 已连接的业务软件 + 每一步敏感操作都要你点头」收。

早期试用者里，官方还引用了三个人：房产经纪 Jess 说它主动发现日历上的看房日写错了；南佛州一家约 110 人餐厅的老板 Amin 用它做账、客服和营销，不用开一百个标签页；品牌策略师 Mya 说它在通话前准备了简报，还发现这场通话紧挨着航班，主动提出改时间。这些是官方文章里的转述。

## **四、哪些用户能使用 Claude Duet**

帮助中心的资格是三条同时满足，少一条现在都进不去：

1. **Claude Pro 或 Max。** 研究预览包含在这两档里，不再另收费。Free 要先升级。
2. **Claude 账号在美国。** 帮助中心原文是 “A Claude account in the US”，看的是这个账号的地区，不是你人在哪里上网。国内代充只把 Free 升成 Pro，地区保持原样。
3. **候补邀请邮件。** 先在产品页提交 Join the waitlist，Anthropic 分批发邮件。邮件到了，按步骤安装并用同一个邮箱登录，才算拿到资格。交了 Pro 或 Max 的钱，不会自动变成这封邀请。

| 账号 | 研究预览能不能用 Duet |
| --- | --- |
| Free | 不能。先要有 Pro 或 Max |
| Pro（美国） | 可以申请候补，邀请分批发 |
| Max（美国） | 可以申请候补，邀请分批发 |
| Team | 还不能，官方说以后会加 |
| Enterprise | 还不能，官方说以后会加 |
| 美国以外 | 研究预览阶段不能 |

费用和额度，按帮助中心 2026-10-21 的说明：

- **不再单独加价。** 研究预览包含在 Pro 和 Max 里。
- **和普通 Claude 共用额度**，包括 5 小时会话额度和周额度，消耗速率和普通对话相同。
- 早报、后台巡检也算额度，所以同样的套餐，开了 Duet 之后可能更早触顶。
- 被接纳进研究预览时，有**一次完整的额度重置**（5 小时额度和周额度都重置）。这次重置可用到 **2026-11-30**。

加入候补不等于有确定日期。邀请是一波一波发的。候补邮箱必须和 Claude 账号一致；手机上如果用 Google 或 Apple 登录，也要是这同一个邮箱，资格绑在这个地址上。

## **五、怎么加入候补，拿到资格后先检查什么**

### 加入候补

按帮助中心的步骤：

1. 打开 [Claude Duet 产品页](https://claude.com/product/claude-duet)，点 **Join the waitlist**。
2. 填写名字和邮箱。已经有 Claude 的，填 Claude 账号那个邮箱。
3. 选你的 Claude 套餐（Pro 或 Max），以及手机是 iPhone 还是 Android。可以再写你做什么工作、第一件想交给它的事。
4. 点 **Submit**。官方是分批加人，轮到你时发邮件。
5. 轮到之后，在手机上打开邀请邮件，按 iPhone 或 Android 的安装步骤走。登录用的 Apple / Google 账号要和候补邮箱是同一个。
6. 打开 Claude Duet，用 Claude 账号登录。接受邀请后，App 可能要过几分钟才出现。

先看官方介绍，弄清它什么会自己做、什么必须等你：[Introducing Claude Duet](https://claude.com/resources/articles/claude-duet)。上手说明在帮助中心：[Get started with Claude Duet](https://support.claude.com/en/articles/17631495-get-started-with-claude-duet)。

### 拿到资格后，先看这三处设置

Duet 从第一条消息就继承 Claude 账号里的记忆、Skills 和 Connectors，基本不用重配。所以进 Duet 之前，先在 Claude 里把这三样收干净：

1. **记忆**：打开 [claude.ai/settings/memory](https://claude.ai/settings/memory)。Duet 会搜索你在 Duet 里的聊天，以及 Claude 里项目以外的历史聊天，用来接着上次的上下文。不想让它翻旧聊天，就把 **Search and reference chats** 关掉。删掉的聊天会从搜索里去掉。
2. **Skills**：你在 Claude 里已经写好的技能会带过去。只留你愿意让一个「会主动开工」的助手使用的技能。
3. **Connectors**：在 Claude 的设置里管理。连接是你自己点的，随时可以断开。断开之后，Duet 不能再访问这个应用；之前对话里已经记住的内容还会留着。

第一次使用，优先让它做「读、整理、起草」。发信、付款、签字、删除，都等它把原文或金额亮出来再点批准。

## **六、国内怎么订阅 Claude Pro / Max**

Duet 不单独卖。没有 Pro 或 Max，候补也进不去。官方订阅要境外卡，国内卡经常被拒，自己绑卡也容易踩风控。本站的做法是卡密代充：支付宝或微信付款，只提交用户 ID，不提交密码。

> **Claude Pro 代充**：[https://littlemagic8.github.io/gptplus/purchase-claude.html](https://littlemagic8.github.io/gptplus/purchase-claude.html)
>
> 自助系统充的是 **Pro**。要 **Max** 请联系 aicygg888，不要用 Pro 卡密去硬充。
>
> 更完整的图文在这里：[一分钟搞定 Claude Pro 充值](https://littlemagic8.github.io/2026/08/16/how-to-sub-claudepro/)。

> **风险说明：** 近期国内不少 Claude 账号被官方风控封禁，和代充无关。封号后订阅一般不退。不能接受这个风险，请不要下单。

### 准备工作

1. 一个能登录 [claude.ai](https://claude.ai) 的账号，状态必须是 **Free**。
2. 打开 [claude.ai/settings/account](https://claude.ai/settings/account)，复制 **Organization ID / 用户 ID**。要 ID，不要密码，也不要填团队 ID。
3. 手机上有支付宝或微信。

### 第一步：购买卡密

打开代充页，点「选购套餐 / 立即购买」，选 **Claude Pro 充值**，不要选「普通账号」。微信或支付宝付款后，系统发货，里面有卡密和充值系统地址。

![Claude Pro 专业代充服务页](/img/2026-08-16-how-to-sub-claudepro/pro-recharge.png)

![选择 Claude Pro 充值套餐](/img/2026-08-16-how-to-sub-claudepro/buy-account.png)

### 第二步：复制用户 ID

在已经登录 claude.ai 的同一个浏览器里打开账户设置，复制那一长串 ID。它不是邮箱。

![在 Settings → Account 复制用户 ID](/img/2026-08-16-how-to-sub-claudepro/org-id.png)

### 第三步：核销卡密

打开发货信息里的充值系统。页面打不开时，先关掉梯子。粘贴卡密并验证，再把用户 ID 贴进去，确认升级。一般 **2～10 分钟**到账。

![打开 Claude 充值系统，先验证卡密](/img/2026-08-16-how-to-sub-claudepro/recharge.png)

![验证卡密后填写用户 ID](/img/2026-08-16-how-to-sub-claudepro/get-userid.png)

充之前对一下：

| 情况 | 能不能充 |
| --- | --- |
| 账号是 Free | 可以 |
| 还在 Pro 或其它订阅期内 | 等过期变回 Free |
| 团队账号，或填了团队 ID | 不行，要用个人用户 ID |
| Billing 有欠款，或还绑着卡 | 先取消自动续费、删掉其它付款方式、结清欠款 |
| 要 Max | 联系 aicygg888，不要用 Pro 卡密 |

### 第四步：确认 Pro 到账，再去排队

头像 → Settings → Account / Billing，显示 **Pro** 就是到账。还显示 Free 的话，退出再登录。仍然不对，把订单号和用户 ID 发给 aicygg888。

![到账后相当于开通了 Subscribe to Pro 这一档](/img/2026-08-16-how-to-sub-claudepro/upgrade-2.png)

Pro 到账之后，回到 [Duet 产品页](https://claude.com/product/claude-duet) 用**同一个邮箱**加入候补，等官方邀请邮件。帮助中心写的是 “A Claude account in the US”：账号本身要在美国。代充只负责订阅，账号地区还是原来的地区，邀请也要自己等。账号不在美国，这一阶段官方不开放。

## **七、使用前看清的安全边界**

官方把这几条写成产品设计，不是使用建议：

- **它不会直接看到你的密码。** 网站要登录时，你在自己设备上的单独表单里输入，密码进浏览器，设计上不进和 Duet 的聊天。凭证处理沿用 Claude Managed Agents 那套。
- **有一个新的分类器专门看外发内容。** 信用卡号、政府证件这一档，设计上会拒绝分享。健康、个人财务这类信息，只有你明确让它发送时才放行。
- **重要决定留在你手里。** 发消息、付款、签字、删除，都要先给你看即将执行的内容。
- 即使用户批准，交易证券、账户间转账、进入他人账号，仍然不做。
- 它会读别人写的邮件和网页，这些内容里可能夹着提示注入。官方说没有任何防护是完美的，所以后果大的操作仍然要你点头。
- 红队和外部机构做过渗透测试，并纳入 Anthropic 的公开漏洞赏金。

你可以随时断开任何一个它能访问的应用。

## **总结**

Claude Duet 是 Claude 第一次做成「会先来找你」的个人智能体：早上简报、你不在也继续做、敏感操作先问你。模型是 Opus 5.5，记忆和已连接的应用从现有 Claude 账号带过去。

现在能用的人，要同时是 Pro 或 Max、Claude 账号在美国，并且已经收到候补邀请邮件。它包含在 Pro 和 Max 里，不再另收费，但后台巡检会计入原有额度。Free、Team、Enterprise，以及不在美国的账号，研究预览还进不去。

国内如果要先把账号升到 Pro，用本站卡密代充，只交用户 ID。升到 Pro 只满足三件里的一件，账号地区不变，还要自己去产品页排队等邀请。Max 直接联系 aicygg888。

## 联系我们

充值过程中遇到任何问题，或有其他业务需求，请联系我们。

请保存网址 [https://littlemagic8.github.io/gptplus/](https://littlemagic8.github.io/gptplus/) ，并加上联系方式，防止失联。

防失联客服微信：

```
aicygg888
```

添加好友请备注：**Claude代充**（加的人多，微信防频繁，请扫码）

## 小提示：想用更多 AI 产品，可以联系 V: aicygg888

> **如果不想开通信用卡，可参考：无需开通信用卡完成 ChatGPT 订阅教程。**
>
> ChatGPTplus 独享账号升级充值自助平台：[https://littlemagic8.github.io/gptplus/](https://littlemagic8.github.io/gptplus/)（网站下方有购买卡密和使用教程）
>
> GPT 代充直达：[https://littlemagic8.github.io/gptplus/purchase-gpt.html](https://littlemagic8.github.io/gptplus/purchase-gpt.html)（支付宝/微信付款，几分钟到账，无需账密）
>
> Claude Pro 代充直达：[https://littlemagic8.github.io/gptplus/purchase-claude.html](https://littlemagic8.github.io/gptplus/purchase-claude.html)
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
