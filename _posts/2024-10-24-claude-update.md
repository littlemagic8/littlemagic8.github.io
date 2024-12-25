---
layout:     post
title:      Claude HaiKu模型介绍和如何获取Claude Pro教程
subtitle:   Claude Pro升级使用教程和HaiKu模型介绍
date:       2024-10-23
author:     aicygg888
header-img: img/claude1.png
catalog: true
tags:
    - Claude
---

## **前言**

anthropic 宣布推出**升级版 Claude 3.5 Sonnet**和新型号**Claude 3.5 Haiku**。升级版 Claude 3.5 Sonnet 比其前代产品有了全面改进，在编码方面取得了显著进步，而编码在这一领域已经处于领先地位。在多次评估中，Claude 3.5 Haiku 的性能与我们之前最大的型号 Claude 3 Opus 相当，价格相同，速度与上一代 Haiku 相近。

我们还将推出一项突破性的新功能：**计算机使用**。[从今天起，开发人员可以通过 API](https://docs.anthropic.com/en/docs/build-with-claude/computer-use)控制 Claude 以人类的方式使用计算机——查看屏幕、移动光标、单击按钮和输入文本。

## **正文**

2024 年 10 月 22 日●阅读时间： 5 分钟

![克劳德操作电脑光标的插图](https://www.anthropic.com/_next/image?url=https%3A%2F%2Fwww-cdn.anthropic.com%2Fimages%2F4zrzovbb%2Fwebsite%2Fdb3165778de297272875d36a822f671d8009aaec-2880x1620.png&w=3840&q=75)



今天，我们宣布推出**升级版 Claude 3.5 Sonnet**和新型号**Claude 3.5 Haiku**。升级版 Claude 3.5 Sonnet 比其前代产品有了全面改进，在编码方面取得了显著进步，而编码在这一领域已经处于领先地位。在多次评估中，Claude 3.5 Haiku 的性能与我们之前最大的型号 Claude 3 Opus 相当，价格相同，速度与上一代 Haiku 相近。

我们还将推出一项突破性的新功能：**计算机使用**。[从今天起，开发人员可以通过 API](https://docs.anthropic.com/en/docs/build-with-claude/computer-use)控制 Claude 以人类的方式使用计算机——查看屏幕、移动光标、单击按钮和输入文本。Claude 3.5 Sonnet 是首个提供计算机使用功能的前沿 AI 模型，目前处于公开测试阶段。目前，它仍处于[试验](https://www.anthropic.com/news/developing-computer-use)阶段——有时很繁琐且容易出错。我们提前发布了计算机使用功能，以征求开发人员的反馈，并预计随着时间的推移，该功能将迅速改进。

Asana、Canva、Cognition、DoorDash、Replit 和 The Browser Company 已经开始探索这些可能性，执行需要数十步甚至数百步才能完成的任务。例如，Replit 正在利用 Claude 3.5 Sonnet 的计算机使用和 UI 导航功能来开发一项关键功能，该功能可在为其 Replit Agent 产品构建应用程序时对其进行评估。

<iframe frameborder="0" allowfullscreen="" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" title="Claude | 使用计算机实现自动化操作" width="100%" height="100%" src="https://www.youtube-nocookie.com/embed/ODaHJzOyVCQ?autoplay=0&amp;mute=0&amp;controls=1&amp;origin=https%3A%2F%2Fwww.anthropic.com&amp;playsinline=1&amp;showinfo=0&amp;rel=0&amp;iv_load_policy=3&amp;modestbranding=1&amp;enablejsapi=1&amp;widgetid=3" id="widget4" data-gtm-yt-inspected-10="true" style="box-sizing: inherit;"></iframe>

升级版 Claude 3.5 Sonnet 现已面向所有用户开放。从今天开始，开发人员可以使用 Anthropic API、Amazon Bedrock 和 Google Cloud 的 Vertex AI 上的计算机使用测试版进行构建。新版 Claude 3.5 Haiku 将于本月晚些时候发布。

![img](https://www.anthropic.com/_next/image?url=https%3A%2F%2Fwww-cdn.anthropic.com%2Fimages%2F4zrzovbb%2Fwebsite%2F0eb9a1b7d5db74a6d21500e9f188c83beef3842e-2601x1932.png&w=3840&q=75)

### Claude 3.5 Sonnet：业界领先的软件工程技能



升级后的[Claude 3.5 Sonnet](https://www.anthropic.com/claude/sonnet)在行业基准测试中表现出广泛的改进，在代理编码和工具使用任务方面尤其取得了显著的进步。在编码方面，它在[SWE-bench Verified](https://www.swebench.com/)上的性能从 33.4% 提高到了 49.0%，得分高于所有公开可用的模型——包括 OpenAI o1-preview 等推理模型和专为代理编码设计的系统。它还在零售领域将代理工具使用任务[TAU-bench](https://github.com/sierra-research/tau-bench)的性能从 62.6% 提高到了 69.2%，在更具挑战性的航空领域从 36.0% 提高到了 46.0%。新款 Claude 3.5 Sonnet 以与其前代产品相同的价格和速度提供了这些进步。

早期客户反馈表明，升级后的 Claude 3.5 Sonnet 代表了人工智能编码的重大飞跃。GitLab 对该模型进行了 DevSecOps 任务测试，发现它提供了更强的推理能力（在用例中高达 10%），并且没有增加延迟，使其成为支持多步骤软件开发流程的理想选择。Cognition 使用新的 Claude 3.5 Sonnet 进行自主人工智能评估，与之前的版本相比，在编码、规划和解决问题方面都有了显著的改进。Browser Company 在使用该模型自动化基于 Web 的工作流程时指出，Claude 3.5 Sonnet 的表现优于他们之前测试过的所有模型。

作为我们持续与外部专家合作的一部分，美国人工智能安全研究所 (US AISI) 和英国安全研究所 (UK AISI) 对新款 Claude 3.5 Sonnet 模型进行了联合部署前测试。

我们还对升级版的 Claude 3.5 Sonnet 的灾难性风险进行了评估，发现我们的[负责任的扩展政策](https://www.anthropic.com/news/announcing-our-updated-responsible-scaling-policy)中概述的 ASL-2 标准仍然适用于该模型。

### Claude 3.5 Haiku：先进技术与经济实惠和速度的完美结合



[Claude 3.5 Haiku](https://www.anthropic.com/claude/haiku)是我们最快模型的下一代。在与 Claude 3 Haiku 相同的成本和相似速度下，Claude 3.5 Haiku 在所有技能组合上都有所提升，甚至在许多智能基准测试中超越了我们上一代最大的模型 Claude 3 Opus。Claude 3.5 Haiku 在编码任务上尤其强大。例如，它在 SWE-bench Verified 上的得分为 40.6%，优于许多使用公开可用的最先进模型的代理——包括原始的 Claude 3.5 Sonnet 和 GPT-4o。

Claude 3.5 Haiku 具有低延迟、改进的指令跟踪和更准确的工具使用功能，非常适合面向用户的产品、专门的子代理任务，以及从海量数据（如购买历史、定价或库存记录）中生成个性化体验。

Claude 3.5 Haiku 将于本月晚些时候在我们的第一方 API、Amazon Bedrock 和 Google Cloud 的 Vertex AI 上推出 - 最初是作为纯文本模型，随后将提供图像输入功能。

### 教 Claude 负责任地操作电脑



在使用计算机方面，我们正在尝试一些全新的事物。我们不是制作特定工具来帮助 Claude 完成单个任务，而是教它*通用的*计算机技能——允许它使用为人类设计的各种标准工具和软件程序。开发人员可以使用这种新兴功能来自动化重复流程、[构建和测试软件](https://www.youtube.com/watch?v=vH2f7cjXjKI)，以及[开展开放式任务，例如研究](https://youtu.be/jqx18KgIzAE)。

为了实现这些通用技能，我们构建了 API，使 Claude 能够感知计算机界面并与之交互。开发人员可以集成此 API，使 Claude 能够将指令（例如“使用我的计算机和在线数据填写此表格”）转换为计算机命令（例如，检查电子表格；移动光标以打开 Web 浏览器；导航到相关网页；使用这些页面中的数据填写表格；等等）。在[OSWorld](https://os-world.github.io/)（评估 AI 模型像人类一样使用计算机的能力）上，Claude 3.5 Sonnet 在纯屏幕截图类别中的得分为 14.9%——明显优于排名第二的 AI 系统的 7.8%。当提供更多步骤来完成任务时，Claude 的得分为 22.0%。

虽然我们预计这种能力将在未来几个月内迅速提高，但 Claude 目前使用计算机的能力并不完美。人们毫不费力执行的一些操作（滚动、拖动、缩放）目前对 Claude 提出了挑战，我们鼓励开发人员从低风险任务开始探索。由于计算机的使用可能会为垃圾邮件、错误信息或欺诈等更常见的威胁提供新的载体，因此我们正在采取积极主动的方式来促进其安全部署。我们开发了新的分类器，可以识别何时使用计算机以及是否发生了危害。您可以在我们关于[开发计算机使用的](http://anthropic.com/news/developing-computer-use)帖子中阅读有关这项新技能背后的研究过程的更多信息，以及对安全措施的进一步讨论。

### 展望



从这项仍处于早期阶段的技术的初始部署中学习，将有助于我们更好地理解日益强大的人工智能系统的潜力和影响。

我们很高兴您能探索[我们的新模型](https://assets.anthropic.com/m/1cd9d098ac3e6467/original/Claude-3-Model-Card-October-Addendum.pdf)和计算机使用的公开测试版，并欢迎您与我们[分享您的反馈](mailto:feedback@anthropic.com)。我们相信这些发展将为您与 Claude 的合作开辟新的可能性，我们期待看到您的创作。



## **如何注册Claude账号和升级订阅开通Claude Pro**

订阅Claude Pro[教程](https://littlemagic8.github.io/2024/09/24/use-ClaudePro-model/)

https://littlemagic8.github.io/2024/09/24/use-ClaudePro-model/

在开通和使用Claude的过程中，如遇到任何问题，欢迎咨询我！

Claude真的好用但是真的太容易封号了！！！如果你需要镜像账号可以使用下面的参考:[镜像账号](https://littlemagic8.github.io/2024/09/13/GPT-o1-get/)

https://littlemagic8.github.io/2024/09/13/GPT-o1-get/

PS：如果你需要订阅ChatGPTPlus可以参考本文：[ChatGPTPlus升级教程](https://littlemagic8.github.io/2024/09/04/update-ChatGPT-Plus/)https://littlemagic8.github.io/2024/09/04/update-ChatGPT-Plus/)