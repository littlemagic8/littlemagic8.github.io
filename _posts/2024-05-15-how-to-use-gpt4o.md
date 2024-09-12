---
layout:     post
title:      openAI最新GPT-4o模型使用教程和简介
subtitle:   2024年5月最新GPT-4o模型使用教程和简介
date:       2024-05-15
author:     aicygg888
header-img: img/post-bg-cook.jpg
catalog: true
tags:
    - gpt-4o

---

## 前言

前两天，2024 年 5 月 13 日，openai 发布了最新的模型 GPT4o。

很多同学还不知道如何访问GPT-4、GPT-4 Turbo和GPT-4o等模型，这篇文章介绍如何在ChatGPT中访问GPT-4o，以及通过OpenAI API访问GPT-4、GPT-4 Turbo和GPT-4o。

## 正文

# 一、什么是GPT-4o？

GPT-4o是OpenAI的新旗舰模型，能够实时处理音频、视觉和文本。

GPT-4o将首先在ChatGPT和API中作为文本和视觉模型提供（ChatGPT将继续支持通过现有的语音模式功能进行语音交互）。


具体来说，GPT-4o将在ChatGPT的Plus版（付费）和Team版中提供（企业版即将推出），以及在聊天完成API、助手API和批处理API中提供。

# 二、如何使用 GPT-4o？

现在 ChatGPT Plus 用户可以直接使用GPT-4o，感受这一全能AI的强大功能。![image-20240515184755437](E:\typoraPicture\image-20240515184755437.png)

如果你还没有 ChatGPT 账号，可以看这篇文章注册账号: ChatGPT账号注册(opens new window)


如果已经有了 ChatGPT 账号，那么需要升级 Plus，目前国内升级 Plus 最方便快捷的便是，虚拟卡，虚拟卡可以理解为一张充值卡，你把钱充在里面，然后使用它去支付 Plus 费用。

目前用过最好用的虚拟卡平台是 wildcard，网址：

https://wildcard.com.cn/i/DW62 (opens new window)(PS: 邀请码记得填上 DW62，这样有后续信用卡支付会有 2 美元优惠



这个平台最方便的是，可以快速一键升级完你的 GPT 账号，之前我在其它虚拟卡平台购买的卡片信息，需要自己去 openai 官网输入卡账号等信息，还会因为 IP 在国内被拒绝支付，所以这个平台的一键升级就解决了这些问题，非常丝滑～




具体升级 ChatGPT Plus 的详细方法可以看这篇文章: GPT4暂停升级，如何开通 ChatGPT Plus: GPT4、GPT4.0 升级 详细指南(opens new window)


#三 、在OpenAI API中访问GPT-4、GPT-4 Turbo和GPT-4o
GPT-4 Turbo与GPT-4o的区别：

定价：GPT-4o比GPT-4 Turbo便宜50%，输入每百万tokens费用为5美元，输出每百万tokens费用为15美元。
速率限制：GPT-4o的速率限制比GPT-4 Turbo高5倍——每分钟最多可处理1000万个tokens。
速度：GPT-4o比GPT-4 Turbo快2倍。
视觉：GPT-4o在与视觉相关的评估中表现优于GPT-4 Turbo。
多语言：GPT-4o对非英语语言的支持比GPT-4 Turbo有所改善。
GPT-4o当前的上下文窗口为128k，其知识截止日期为2023年10月。

API中的可用性拥有OpenAI API账户的任何人都可以使用GPT-4o模型，您可以在聊天完成API、助手API和批处理API中使用此模型。此模型还支持函数调用和JSON模式。您也可以通过Playground开始使用。

在成功支付5美元或更多（使用等级1）后，您将能够通过OpenAI API访问GPT-4、GPT-4 Turbo和GPT-4o模型。


了解更多关于向您的OpenAI账户添加信用额度的信息。

API当前的GPT-4o定价请参阅我们的API定价页面。

API请求限制请注意，ChatGPT的速率限制独立于API的速率限制。您可以在这里了解更多关于API速率限制的信息。

您可以在API平台的限制部分查看您的API速率限制。

请耐心等待——我们预计会有大量需求，并将在未来几个月内扩大和优化我们的系统。

我们如何处理发送到OpenAI API的数据

与我们平台的其他部分一样，除非您明确选择参与训练，否则通过OpenAI API传输的数据和文件不会用于训练我们的模型。您可以在此处阅读更多关于我们的数据保留和合规标准的信息。


在ChatGPT中访问GPT-4oChatGPT免费版

免费版用户将默认使用GPT-4o，但对使用GPT-4o发送的消息数量有限制，该限制会根据当前使用情况和需求而变化。当不可用时，免费版用户将切换回GPT-3.5。

免费用户还可以有限制地访问使用高级工具发送的消息，例如：

数据分析
文件上传
浏览
发现和使用GPT模型
视觉
GPT-4o具有高级的视觉能力，提高了对您分享的图像的理解准确性。


免费版用户可以随时通过点击ChatGPT升级到Plus版。



#四、ChatGPT Plus和Team

ChatGPT Plus和Team订阅者在chatgpt.com上可以访问GPT-4和GPT-4o，并有更大的使用限制。

ChatGPT Plus和Team用户可以通过页面顶部的下拉菜单选择GPT-4o。



从2024年5月13日起，Plus用户每3小时可以发送最多80条使用GPT-4o的消息和最多40条使用GPT-4的消息。在高峰时段，我们可能会减少限制，以使GPT-4和GPT-4o能被更多人访问。

ChatGPT Team工作区用户的GPT-4和GPT-4o消息上限高于ChatGPT Plus用户。

请注意，未使用的消息不会累积（即如果您等待6小时，您在接下来的3小时内仍然只能使用80条GPT-4的消息）。

#五、ChatGPT企业版
ChatGPT企业版客户将很快能够访问GPT-4o。

ChatGPT企业版计划专为满足大型企业的需求而设计，提供无限制、高速访问GPT-4o和GPT-4。

企业账户上的新对话将默认使用GPT-4o。ChatGPT企业用户可以通过页面顶部的下拉菜单选择其他模型。



ChatGPT企业版还提供企业级的安全和隐私、更长的上下文窗口以处理更长的输入、无限制的高速访问高级工具如数据分析、定制选项等等。

作者: 编程指北
链接: https://csguide.cn/private/how-to-use-gpt4o.html
来源: https://csguide.cn
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。