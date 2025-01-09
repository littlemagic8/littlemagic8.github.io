---
layout:     post
title:      （2025最新）国内如何充值OpenRouter的教程，国内稳定访问OpenAI API 和 Claude3.5 API 的方式
subtitle:   国内稳定访问OpenAI API 和 Claude3.5 API 的方式【2025年 最新更新】
date:       2025-01-10
author:     aicygg888
header-img: img/post-bg-cook.jpg
catalog: true
tags:
    - API
---

## OpenRouter是什么？

相信很多朋友需要对接OpenAI的**ChatGPT API**、Anthropic公司下的**Claude API** 或者 **Google aistudio API**，而这些API在国内有个**缺点**，就是**不能直接调用**。

特别是Claude对环境要求非常严格，如果不纯净就会出现被封的情况。

**有没有一个不受限制，不用担心被封号的，可以在国内稳定访问并提供api支持的方式呢？**

答案自然是有的，比如**OpenRouter**，如下图：

![img](https://picx.zhimg.com/80/v2-fc630061393c4fbf8c5f3eb4bd0079ab_720w.png)



刚好最近比较火的IDE插件：Cline3.1。目前调用量也是排名第一，使用过Cursor的用户，可以了解一下Cline3.1最新更新。

而对应的**LLM API调用量排名依据是Claude3.5** **sonnet 排名第一。**

Claude 3.5 -> Gemini Flash 1.5 -> DeepSeek V3 (国货开源之光)

![img](https://pic1.zhimg.com/80/v2-0aa635b0633209b2bb189149ff72c3c2_720w.png)

回到主题，**而OpenRouter提供了可以在国内直接方便访问的方式**，而且不仅有OpenAI的GPT-4o、o1、 Anthropic的Claude3.5 Sonnet、Google aistudio API，还支持多个其它企业的大模型。

OpenRouter 为 293 个模型和提供者提供了兼容 OpenAI 的 API，你可以直接调用或使用 OpenAI SDK。另外，OpenRouter也还提供一些第三方 SDK。

```
from openai import OpenAI

client = OpenAI(
  base_url="https://openrouter.ai/api/v1",
  api_key="<OPENROUTER_API_KEY>",
)

completion = client.chat.completions.create(
  extra_headers={
    "HTTP-Referer": "<YOUR_SITE_URL>", # Optional. Site URL for rankings on openrouter.ai.
    "X-Title": "<YOUR_SITE_NAME>", # Optional. Site title for rankings on openrouter.ai.
  },
  model="openai/gpt-3.5-turbo",
  messages=[
    {
      "role": "user",
      "content": "What is the meaning of life?"
    }
  ]
)
print(completion.choices[0].message.content)
```

你可以设置OpenRouter的默认模型，也就是当你没有积分时，可以调用一些免费的LLM API，比如谷歌的Gemini 2.0 Flash API。

**点击头像 -> Settings -> Default Model 中进行设置。**

![img](https://picx.zhimg.com/80/v2-f783cec291b1945abea785640d0f529a_720w.png)



Default Model选择你需要的模型

![img](https://pic1.zhimg.com/80/v2-24a11246a46b854bd369476b41be70f4_720w.png)





## 一、充值 Credits 和 充值 OpenRouter的方法

当你需要使用一些需要消耗Credits（积分）的LLM API时，就需要你对OpenRouter进行充值，充值方法也不难。

点击头像 -> Credits -> 点击 Open Billing Portal 就可以进行充值。

![img](https://picx.zhimg.com/80/v2-0133835062c13c8dcb9b268654b08756_720w.png)





> **PS:在充值之前需要绑卡哦，可以使用**[**虚拟卡**](https://bewildcard.com/i/DW62)**（**[**https://bewildcard.com/i/DW62**](https://bewildcard.com/i/DW62)**），笔者也是使用这种方式，待会我会详细介绍绑卡过程
> **虚拟卡申请教程：[卡片申请教程](https://littlemagic8.github.io/2024/12/23/how-to-use-wildcard/)

![img](https://picx.zhimg.com/80/v2-e3dca58527077c84fe60a187042044a6_720w.png)



**它还支持Crypto的方式！知道加密货币的小伙伴，应该就知道怎么进行这种方式进行充值。**

不过需要点击开启之后，才能进行操作。

![img](https://pic1.zhimg.com/80/v2-25785ba58375c07178bf1e1f4bc51989_720w.png)







## 二、国内充值OpenRouter的方式

同样也是进入到Credits页面，如果你还没有绑定卡号的，可以先绑定卡号再进行充值对应的积分，也可以直接点击Add Credits 进行绑卡并且充值积分。

![img](https://pica.zhimg.com/80/v2-cceea631ae0a281ba0202da9a7b4d265_720w.png)





**注意：这里的卡号，需要国际的visa、master类型的卡！！！**

如果没有这种类型的卡的话，可以申请一张虚拟海外卡，我当前使用的虚拟卡是bewildcard。如果你也需要可以通过官网进行申请一张，目前是2年10.9刀乐的年费。 （**我之前是1年9.9刀乐**）

> **虚拟卡官网入口：** [卡片](https://bewildcard.com/i/DW62)

开通申请之后，就可以获得对应的卡号信息和地址。（有了虚拟visa卡，就可以搞定很多事情啦！）

![img](https://picx.zhimg.com/80/v2-62fb8fb23ab811e69a091265fc9dfff1_720w.png)



对了，虚拟卡充值时，你需要用多少充值多少就行！**虽然它可以秒提现、也支持国内支付宝的充值方式，但是为了避免损失，还是用多少充多少！**（目前稳定使用了1年多的时间吧）

## 三、绑卡教程

### 绑卡方式一

有了卡号之后，就可以直接到OpenRouter进行一个绑卡操作，点击添加支付方式。**选择**”银行卡“

![img](https://pic1.zhimg.com/80/v2-55d1c2e4c00f245867fd399765cf6910_720w.png)



接着把你的卡号信息填入到这边来，就可以进行一个绑定。 **（建议在绑定之前，可以先充值好6刀到虚拟卡余额上）**

![img](https://picx.zhimg.com/80/v2-ced08f7cd81dc002951909c0f55bf95a_720w.png)



**绑定时，会出现验证报错时，不用着急！重新绑定一下即可，同时检查一下当前的网络是否稳定。**

下面就是绑定成功之后的情况，就可以进行一个充值OpenRouter的积分啦。当然了，你需要保证你的卡有余额，如果没有余额，你可以通过支付宝进行一个充值。

![img](https://pic1.zhimg.com/80/v2-89767bdfbf43ff3a812ffb5b3593554f_720w.png)



**添加完毕之后，别忘记，顺便把账单地址也补充一下，填写你的虚拟卡的卡号信息里的地址。**

![img](https://picx.zhimg.com/80/v2-fe3b993608d6f0c142a9ae9ecbbf11f7_720w.png)



### 绑卡方式二（推荐）

直接点击【Add Credits】进行绑卡，就不会出现一些需要验证邮箱地址的相关问题。

![img](https://pic1.zhimg.com/80/v2-59f5223f3e72b86da159b21176acbc32_720w.png)



绑定之后的，OpenRouter的验证，你的卡片会收到这条记录，就表示OpenRouter和你的虚拟卡已经绑定成功，OpenRouter使用了一个预扣款的方式。

![img](https://pic1.zhimg.com/80/v2-fbb67a2ed033bb6ce2553442bdff9e39_720w.png)







## 四、相关报错解决方式

**报错：you must have a verified email address for this feature.**

接着，你就可以进行一个Credits充值，如果你点击【Add Credits】时，出现了下面的错误时，不用着急！

![img](https://pica.zhimg.com/80/v2-464bf88d864002a3fe119d7c714bb8b3_720w.png)

### 解决方式一：

1. 通过增加多一个邮箱就解决了。
2. 完善了账单地址（填上虚拟卡号上的地址）

接着重新登录就可以解决了。

点击setting->Account->Manage Account 如下图所示：

![img](https://pic1.zhimg.com/80/v2-62fbc1a711bfede9530c0bd6c0e6e609_720w.png)



### 解决方式二：

**你还没有绑卡的情况下**，添加卡时，直接点击【Add Credits】进行验证账单地址，然后进行绑卡。

![img](https://picx.zhimg.com/80/v2-5e5bfef99738dc50aee8e53345d519a1_720w.jpg)

成功绑定，并且能跳出下面的窗口，就可以进行选择对应的卡，进行一个充值。

![img](https://picx.zhimg.com/80/v2-51028805350ca75d7f95eb799effd3f3_720w.png)







而Openrouter最低充值是5刀，所以你一定要确保虚拟卡的余额已经有6刀左右。否则可能导致支付失败

![img](https://picx.zhimg.com/80/v2-6b67f5111700ad5d6b350f77e3d9898c_720w.png?source=d16d100b)

好了，这就是整个OpenRouter的充值流程教程，操作大概10分钟左右完成了。

# 结论

OpenRouter 有许多优点

1. 支援多种热门的AI 模型，使用者可以根据需求选择最适合的模型。
2. 由于透过单一的API，使用者可以与多个模型交谈，无需为不同模型设计不同的介面。
3. 提供不少免费的大语言模型，节省经费也能达到测试开发目的。

本篇分享结束，希望大家透过语言模型开发顺利，有机会再多分享开发工具。





### **小提示：**

>  ** PS:如果你需要开通自己的ChatGPT Plus、Claude Pro的个人独享账号可以参考教程：**[使用支付方式订阅开通ChatGPT Plus、Claude Pro教程](https://littlemagic8.github.io/2024/12/09/ChatGPT-and-Cluade/)

> **PS：如果你想使用镜像账号可以参考本文** [镜像账号](https://littlemagic8.github.io/2024/09/13/GPT-o1-get/)
>
> **或者微信加我获取 aicygg888**

欢迎加微信

![img](https://picx.zhimg.com/80/v2-b1c8f90bffc8b2f4f32ab07a08a4ede6_720w.png)

公众号也可以哦

![img](https://pic1.zhimg.com/80/v2-4e622b64238b20948a02e0c988ca5704_720w.png)