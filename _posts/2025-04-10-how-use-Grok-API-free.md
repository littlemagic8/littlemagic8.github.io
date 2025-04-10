---
layout:     post
title:      如何白嫖Grok3 API？如何使用Grok3 API调用实例？怎么使用Grok3模型
subtitle:   白嫖Grok3 API
date:       2025-04-10
author:     aicygg888
header-img: img/post-bg-cook.jpg
catalog: true
tags:
    - grok
---

## **前言**

前段时间，Grok3（**想要体验Grok3的童鞋可以参考本文：**https://littlemagic8.github.io/2025/03/19/Grok-3-role/）一经发布就排到了竞技场第一，当时Grok3 API并没有开放，今天Grok3 API 现在已经官宣全网上线使用，只要需要绑定卡并且充值不低于5美金并开启数据共享就可以免费使用Grok3 API了。

![img](https://pic1.zhimg.com/80/v2-06d4e96702d63e0e89143018f0ba0341_720w.png)

**grok-3-beta和grok-3-mini-beta 现在可用，支持文本模式，上下文窗口为131072 tokens**

**定价（每百万tokens）：**

- grok-3-beta，输入：3.00美元，输出：15.00美元
- grok-3-mini-beta，输入：0.30美元，输出：0.50美元

![img](https://pic1.zhimg.com/80/v2-a24002c1637c7e74a653cbc894044a05_720w.png)

**另外两个模型还支持了对应的fast版本，也就是请求速度和响应更快，但是价格也更高。**

虽然API目前处于beta阶段，但xAI计划频繁更新Grok 3模型，并可能在未来添加更多功能，例如本次的推理和图像生成已经上线支持了。

## **怎么免费使用Grok3 API**

教程开始之前，肯定得先知道Grok API平台，并且注册一个账号，**建议使用“谷歌邮箱”登录，** 下面就是Grok API 开发者平台："console.x.ai"

**那么如何才可以薅到Grok API 的 150美元体验金呢？有个前置条件：**

- 绑定支付卡片，并充值最低 5 美元
- 加入数据共享计划

![img](https://pic1.zhimg.com/80/v2-be0efa11243eae4fded6748dc521e314_720w.png)

## **国内如何绑卡并充值 Grok API 5 美元呢？**

### 第一步：申请卡片

如果你有国内的visa、master国际信用卡，也可以尝试。**如果不行，或者没有国际信用卡的话，就使用Master虚拟卡。**

> **Master虚拟卡**：*https://littlemagic8.github.io/pay/*

申请之后，会有一个美区的Master国际信用卡信息，可以把这些信息进行绑定 X AI 平台，也就是 Grok API 平台。

![img](https://pica.zhimg.com/80/v2-7a45ad2c80162fb16c44acea59a3c75a_720w.png)

### 第二步：充值卡片

先给虚拟卡充值5美刀，可以使用支付宝进行充值，不使用的话，可以直接提现。

![img](https://picx.zhimg.com/80/v2-02aa07d4260c017e6d97ac2a04c2bc2a_720w.png)

**绑卡时，注意使用的魔法建议纯净度良好的，自测方式：ping0.cc。 绑定时，被拒的原因，大部分是网络环境问题。**

### 第三步：填写账单地址、绑卡

打开 Grok API 平台：“console.x.ai” 按下面，找到 “Payment settings” 进行 填写账单地址，然后再添加卡。

这两个信息都直接用虚拟卡上的信息即可。**虚拟卡上没有的信息，可以不用填，比如 最下方的电话号码。**

![img](https://pic1.zhimg.com/80/v2-1dac98cc8fbbc8efced562494e627fb6_720w.png)

填完账单地址之后，就可以进行绑卡了，绑定之后，充值 5 美元即可。

![img](https://pic1.zhimg.com/80/v2-d27fda5e3bcbca9607133235317b5ad3_720w.png)

这里，我使用的魔法节点是美区｜原生｜IP，纯净度还可以。就直接一次性过了，不通过的情况下，可以重试哈。

![img](https://picx.zhimg.com/80/v2-5b7b488caaf2ef0e82d5e287c24de129_720w.png)



![img](https://pic1.zhimg.com/80/v2-308db9f4ebe682fc5b1f3d5eb9b961ce_720w.png)



### 第四步：绑定成功提示

绑定成功之后，有一条预扣款 0 元的信息：

![img](https://picx.zhimg.com/80/v2-c749469632f6420ea52dd5365ca99a9f_720w.png)

### 第五步：使用绑定的卡片支付5美元

确保自己的虚拟卡账户有 5 美元，**最后一步：现在你可以进行一个充值5美元的操作了。**

找到 “Credits”，然后往下滑动， 找到 “Purchase credits” 进行支付即可。

![img](https://pic1.zhimg.com/80/v2-aca5aa789e6445618aa2a892adbe2a63_720w.png)

成功之后，开启数据共享协议，就可以有下面这个150美元的免费额度啦～

![img](https://pic1.zhimg.com/80/v2-853662592924705c67a6b62b35316c6d_720w.png)

### 第六步：签署数据共享协议

如果，你充值了 5 美元之后，还没有到账 150 美元的话，可以来这里查https://console.x.ai/team/default/billing/credits，因为**需要签署一个数据共享协议**:

**关于数据共享协议详细信息可以参考**：https://docs.x.ai/docs/data-sharing#how-it-works

![img](https://picx.zhimg.com/80/v2-4fd47902a985dc91e24f663a59e9efef_720w.png)



![img](https://picx.zhimg.com/80/v2-525978f1570f0a6ff10ad3ce1a8d5b89_720w.png)

你充值5美元之后，在下方测试是否有资格的，可以点击 “check for eligibility“ 就行，之后再到 ”credit“ 里面选择共享数据就可以获得150美元的额度：

![img](https://pic1.zhimg.com/80/v2-7b93f0f20a7525ebef6e012b9f9b9c43_720w.png)

而虚拟卡的话，使用这个 https://littlemagic8.github.io/pay/ 的就行，比较稳定，用了一年多。

### 第七步：这个卡片还能来干什么，支持支付哪些服务？

还可以用来升级订阅SuperGrok 或者 Claude 和 ChatGPT 这些服务～

> ***\*支持的服务(最常问的)： ChatGPT/OpenAI API Claude/Anthropic API Apple Store(美区) Google Play(美区)**

> **Youtube Cursor（需美国网络全局模式） Windsurf/Github Microsoft Azure/Store Poe Suno（需美国网络全局模式） Patreon/pixivFanbox CloudFlare**

> **OpenRouter Facebook**

> **Perplexity MidJourney Telegram（对网络有要求） X/Twitter/Grok Netflix/Hulu/Spotify**

> **AWS(需自己解决地址证明)**

## **推理模型API使用实例**

Grok 3 Mini 是一款轻量级、体积更小的思维模型。与传统的即时生成答案的模型不同，Grok 3 Mini 会先思考后响应。它非常适合处理推理能力强、不需要广泛领域知识的任务，并且在数学特定和定量用例（例如解决具有挑战性的谜题或数学问题）中表现出色。

> PS:推理仅由grok-3-mini-beta和grok-3-mini-fast-beta.Grok 3 型号grok-3-beta和grok-3-fast-beta不支持推理。

### 主要特点

- **三思而后行**：在给出答案之前，逐步思考问题。
- **数学和定量优势**：擅长数字挑战和逻辑谜题。
- **推理轨迹**：模型的想法可以通过reasoning_content响应完成对象中的字段（见下面的示例）。

您可以通过以下方式访问模型的原始思维轨迹message.reasoning_content聊天完成响应。

### 控制模型的思考程度

这reasoning_effort参数控制模型在响应之前花费的思考时间。必须将其设置为以下值之一：

- **low**：最短的思考时间，使用更少的令牌进行快速响应。
- **high**：最大化思考时间，利用更多令牌解决复杂问题。

选择正确的级别取决于你的任务：使用low对于应该快速完成的简单查询，以及high对于响应延迟不太重要的较难问题。

### 使用实例

这是一个使用 Grok 3 Mini 将 101 乘以 3 的简单示例。请注意，我们可以访问推理内容和最终响应。

```
import os
from openai import OpenAI

messages = [
    {
        "role": "system",
        "content": "You are a highly intelligent AI assistant.",
    },
    {
        "role": "user",
        "content": "What is 101*3?",
    },
]

client = OpenAI(
    base_url="https://api.x.ai/v1",
    api_key=os.getenv("XAI_API_KEY"),
)

completion = client.chat.completions.create(
    model="grok-3-mini-beta", # or "grok-3-mini-fast-beta"
    reasoning_effort="high",
    messages=messages,
    temperature=0.7,
)

print("Reasoning Content:")
print(completion.choices[0].message.reasoning_content)

print("\nFinal Response:")
print(completion.choices[0].message.content)

print("\nNumber of completion tokens (input):")
print(completion.usage.completion_tokens)

print("\nNumber of reasoning tokens (input):")
print(completion.usage.completion_tokens_details.reasoning_tokens)
```

### 示例输出

```
输出

Reasoning Content:
Let me calculate 101 multiplied by 3:
101 * 3 = 303.
I can double-check that: 100 * 3 is 300, and 1 * 3 is 3, so 300 + 3 = 303. Yes, that's correct.

Final Response:
The result of 101 multiplied by 3 is 303.

Number of completion tokens (input):
14

Number of reasoning tokens (input):
310
```

### 何时使用推理

- **使用****grok-3-mini-beta****或者****grok-3-mini-fast-beta**：适用于需要逻辑推理的任务（例如会议安排或数学问题）。也适用于不需要特定领域深度知识的任务（例如基本的客户支持机器人）。
- **使用****grok-3-beta****或者****grok-3-fast-beta**：适用于需要深厚领域专业知识或世界知识（例如医疗保健、法律、金融）的查询。

当前API还推出了图像创建等，一次性可以最多创建10张图片，使用"

response = client.images.generate(   model="grok-2-image",   prompt="A cat in a tree" ) "只需要一个简单的一只猫在树上即可得到下面图片：

![img](https://picx.zhimg.com/80/v2-19d2aee43c7f74cc7ad09db32c3d1b99_720w.png)

更多实例可以参考：https://docs.x.ai/docs/overview

END:大家快去把Grok3 API使用起来吧！

## 小提示：

> **PS:如果你需要开通自己的ChatGPT Plus、Claude Pro的个人独享账号可以参考教程：**[**使用支付方式订阅开通ChatGPT Plus、Claude Pro教程**](https://littlemagic8.github.io/2024/09/04/update-ChatGPT-Plus/) 
>
> *PS：国内直接使用chatGPT/Claude镜像账号可以通过两种方式获取：*

方式一：通过教程自行购买：

> *1、*[**镜像账号购买方式1**](https://littlemagic8.github.io/2025/04/10/how-use-share-AI-model/)：https://littlemagic8.github.io/2025/04/10/how-use-share-AI-model/
>
> *2、*[**镜像账号购买参考方式2**](https://littlemagic8.github.io/2024/05/15/how-to-use-ai/) [https://littlemagic8.github.io/2024/05/15/how-to-use-ai/](https://littlemagic8.github.io/2024/05/15/how-to-use-ai/)

不想自己注册账号，可以用方式二

> *方式二：添加微信购买 微信：***aicygg888** *(备注镜像账号哦)*

欢迎加微信

![img](https://picx.zhimg.com/80/v2-46f7cfd62d1e94381388ab08b0fea3af_720w.png)

公众号也可以哦

![img](https://pic1.zhimg.com/80/v2-4e622b64238b20948a02e0c988ca5704_720w.png)
