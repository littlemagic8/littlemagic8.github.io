---

layout:     post
title:      Sora是什么、国内如何使用订阅升级Sora会员保姆级教程
subtitle:   2024年12月最新Sora是什么、国内如何使用订阅升级Sora会员保姆级教程
date:       2024-12-12
author:     aicygg888
header-img: img/openai.jpg
catalog: true
tags:
    - Sora
---

## 前言

Sora震撼发布！！！

支持用提示词修改视频对象，场景不变，一句提示词出四个视频，不同景别，不同运镜，故事版能支持时间线修改视频开始和结尾，人人创作电影的时代到来了！接下来我将从Sora简介和如何使用Sora两个方面进行介绍

## 正文

![img](https://pic1.zhimg.com/80/v2-560bb6bbfe0fdedbe082ecf278ee68c6_720w.webp?source=2c26e567)

## Sora 概述

官网地址：[Attention Required! | Cloudflare](https://sora.com/)

Sora 是 [OpenAI](https://zhida.zhihu.com/search?content_id=703772480&content_type=Answer&match_order=1&q=OpenAI&zhida_source=entity) 的视频生成模型，旨在接收文本、图像和视频输入并生成新视频作为输出。用户可以创建各种格式的分辨率高达 1080p（最长 20 秒）的视频，从文本生成新内容，或增强、混音和融合自己的资产。用户将能够探索精选和最新动态，这些动态展示了社区创作并为新想法提供灵感。

Sora 以 [DALL·E](https://zhida.zhihu.com/search?content_id=703772480&content_type=Answer&match_order=1&q=DALL·E&zhida_source=entity) 和 [GPT 模型](https://zhida.zhihu.com/search?content_id=703772480&content_type=Answer&match_order=1&q=GPT+模型&zhida_source=entity)的经验为基础，旨在为人们提供更多讲故事和创意表达的工具。 Sora 是一种[扩散模型](https://zhida.zhihu.com/search?content_id=703772480&content_type=Answer&match_order=1&q=扩散模型&zhida_source=entity)，它首先从看起来像静态噪声的基础视频开始生成视频，然后通过多个步骤消除噪声，逐渐对其进行转换。通过让模型一次预测多个帧，Sora团队解决了一个具有挑战性的问题，即确保主体即使暂时消失在视野之外也能保持不变。与 GPT 模型类似，Sora 使用 [transformer 架构](https://zhida.zhihu.com/search?content_id=703772480&content_type=Answer&match_order=1&q=transformer+架构&zhida_source=entity)，从而实现卓越的扩展性能。

Sora 使用了 DALL·E 3 中的重新字幕技术，该技术涉及为视觉训练数据生成高度描述性的字幕。因此，该模型能够更忠实地遵循生成的视频中用户的文本指令。 除了能够仅根据文本指令生成视频外，该模型还能够利用现有的静态图像生成视频，以精确的方式对图像内容进行动画处理，并注意细节。该模型还可以利用现有视频进行扩展或填充缺失的帧。

Sora 是理解和模拟现实世界的模型的基础，我们相信这一能力将成为实现 AGI 的重要里程碑。 Sora 的功能还可能带来新的风险，例如可能滥用相似性或生成误导性或露骨的视频内容。为了安全地在产品中部署 Sora，Sora团队借鉴了 DALL·E 在 ChatGPT 中的部署的安全工作以及 ChatGPT 等其他 OpenAI 产品的 API 和安全缓解措施。此系统卡概述了由此产生的缓解堆栈、外部红队工作、评估和正在进行的研究，以进一步完善这些保障措施。

模型数据

正如我们2024 年 2 月的技术报告⁠中所述，Sora 从大型语言模型中汲取灵感，这些模型通过在互联网规模数据上进行训练获得了通才能力。[LLM 范式](https://zhida.zhihu.com/search?content_id=703772480&content_type=Answer&match_order=1&q=LLM+范式&zhida_source=entity)的成功在一定程度上得益于使用标记优雅地统一了各种文本模态——代码、数学和各种自然语言。通过 Sora，我们考虑了视觉数据的生成模型如何继承这些好处。LLM 有文本标记，而 Sora 有视觉补丁。补丁以前已被证明是视觉数据模型的有效表示。我们发现补丁是一种高度可扩展且有效的表示，可用于在各种类型的视频和图像上训练生成模型。在高层次上，我们首先将视频压缩到低维潜在空间，然后将表示分解为时空补丁，从而将视频转换为补丁。 Sora 接受了各种数据集的训练，包括公开数据、通过合作伙伴关系获取的专有数据以及内部开发的自定义数据集。这些数据集包括：

- **选择公开可用的数据**，主要从行业标准的机器学习数据集和网络爬虫中收集。
- **来自数据合作伙伴的专有数据**。我们建立合作伙伴关系来访问非公开数据。例如，我们与 [Shutterstock](https://zhida.zhihu.com/search?content_id=703772480&content_type=Answer&match_order=1&q=Shutterstock&zhida_source=entity)⁠ [Pond5](https://zhida.zhihu.com/search?content_id=703772480&content_type=Answer&match_order=1&q=Pond5&zhida_source=entity) 合作构建和交付 AI 生成的图像。我们还合作委托和创建符合我们需求的数据集。
- **人工数据：**来自 AI 培训师、红队成员和员工的反馈。

## Sora如何使用和订阅

Sora 是 Plus 帐户的一部分，无需额外付费。您每月最多可以生成 50 个 480p 分辨率的视频，或更少的 720p 分辨率的视频。 对于那些想要更多 Sora 的用户，Pro 计划包括 10 倍的使用量、更高的分辨率和更长的持续时间。我们正在为不同类型的用户制定量身定制的定价，Sora计划于明年初推出

![img](https://picx.zhimg.com/80/v2-37a7aad1c60219109ab4720bf47ef6ca_720w.webp?source=2c26e567)

> ***PS: 目前呢Sora是Plus或者Pro的一部分，也就是升级的订阅账户就无需额外付费使用Sora,需要升级的同学可以参考本教程** [ChatGPTPro/plus国内订阅教程](https://littlemagic8.github.io/2024/12/08/how-to-update-ChatGPTPro-plus/)*
> *tips: 目前Sora还需要账户，好像可以用ChatGPT的账号，但是目前是关闭的，大家可以等热度降一降*

![img](https://picx.zhimg.com/80/v2-07adaa6afe43de60fc11d41885a33dc1_720w.webp?source=2c26e567)

*大家可以看看Sora官网发布的视频效果*

![img](https://picx.zhimg.com/v2-58dfc3ebc24f5ed5d77ad587120d827a.jpg?source=25ab7b06)

00:05



![img](https://picx.zhimg.com/80/v2-b839243715738a6e45d5300a044a99d6_720w.webp?source=2c26e567)

*END:大家可以发散自己的脑洞，开始尽情创作了!!!*



### **小提示：**

>  **PS:如果你需要开通自己的ChatGPT Plus、Claude Pro的个人独享账号可以参考教程：**[使用支付方式订阅开通ChatGPT Plus、Claude Pro教程](https://littlemagic8.github.io/2024/12/09/ChatGPT-and-Cluade/)

> **PS：国内直接使用chatGPT/Claude镜像账号可以通过两种方式获取：
>
> > 方式一：通过教程自行购买：
> > [镜像账号购买参考](https://littlemagic8.github.io/2024/05/15/how-to-use-ai/) https://littlemagic8.github.io/2024/05/15/how-to-use-ai/
>
> 不想自己注册账号，可以用方式二
>
> > 方式二：添加微信购买
> > 微信：**aicygg888** (备注镜像账号哦)

欢迎加微信

![img](https://picx.zhimg.com/80/v2-b1c8f90bffc8b2f4f32ab07a08a4ede6_720w.png)

公众号也可以哦

![img](https://pic1.zhimg.com/80/v2-4e622b64238b20948a02e0c988ca5704_720w.png)