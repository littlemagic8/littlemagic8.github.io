---
layout:     post
title:      (2025最新)Claude 3.7 Sonnet怎么样？如何使用Claude 3.7 Sonnet？如何使用Claude Code?如何升级订阅CluadePro
subtitle:   CluadePro使用
date:       2025-02-27
author:     aicygg888
header-img: img/post-bg-cook.jpg
catalog: true
tags:
    - CluadePro
---

![img](https://picx.zhimg.com/v2-83b24b6fd3bd2bdcea386ffb5767e149_1440w.jpg)

最近，Anthropic发布了**Claude 3.7 Sonnet**，这是他们迄今为止最强大的模型，也是市场上首个**混合推理模型**。简单来说，这个模型不仅能快速给出答案，还能像人类一样进行深度思考，特别适合需要复杂推理的任务，比如编码、数学问题解决等。

本文主要介绍了Claude 3.7 Sonnet模型的发布教你如何订阅使用Claude 3.7 Sonnect及其新功能，特别是Claude Code工具的推出。

## Claude本次发布的相关汇总

### **1. Claude 3.7 Sonnet模型**：

Sonnet软件工程得分情况如下 超过目前主流模型，话说为啥没有Grok3(瞧不上20万张的GPU?)

![img](https://picx.zhimg.com/v2-fad47c3df2cbb1e57617382923c489b3_1440w.jpg)

- - 这是Anthropic公司迄今为止最智能的模型，也是市场上首个混合推理模型。
  - 该模型能够生成即时响应或逐步思考的结果，**用户可以通过API控制模型的思考时间**。
  - 在编码和前端开发方面表现出色，特别是在处理复杂代码库和工具使用方面。

### **2. Claude Code工具**：

- - 这是一个命令行工具，允许开发者直接从终端委托工程任务给Claude。
  - 目前处于有限的研究预览阶段，支持搜索、编辑代码、运行测试、提交代码到GitHub等操作。

### **3.** Claude 3.7 Sonnet相关**定价**：

- Claude 3.7 Sonnet在所有Claude计划中可用，包括免费版、**专业版（18刀,一般用户订阅这个就够了）**、团队版和企业版。(注意免费版不能使用扩展思维模式)

![img](https://pica.zhimg.com/v2-d0634cec8677683e754c1e1721b2da30_1440w.jpg)

![img](https://pic4.zhimg.com/v2-ecc96a6f2230b0a3cee4fac65fda8801_1440w.jpg)

> ***PS: 需要体验Claude 3.7 Sonnet Extended thinking mode的童鞋需要升级订阅Claude Pro可以参考本文：\***[国内如何使用支付宝注册Claude账号和升级订阅开通Claude Pro]https://littlemagic8.github.io/2024/09/24/use-ClaudePro-model/)

- - *Claude* API定价为每百万输入token 3美元，每百万输出token 15美元（包括思考token）。

### **4. 模型特点**：

- - Claude 3.7 Sonnet结合了普通LLM和推理模型的功能，用户可以选择模型是快速响应还是深度思考。
  - 在扩展思考模式下，**模型会自我反思后再回答（总之让他自己有思考过程，更像个人）**，显著提升了数学、物理、编码等任务的表现。

### **5. 性能表现**：

Claude 3.7 Sonnet在指令逻辑、一般推理和多模态能力和代码代理能力表现出色，进阶推理在数学和科学有显著的提高，如下图所示

![img](https://pic4.zhimg.com/v2-c0f5be2ba3b524741b6eb4d55b6e3fc7_1440w.jpg)

- - 在多个基准测试中表现优异，特别是在编码、工具使用和多语言问答方面。
  - 在TAU-bench测试中，Claude 3.7 Sonnet在复杂任务中表现最佳。

## 如何使用Claude3.7 Sonnet

Claude 3.7 Sonnet在所有Claude计划中可用，包括免费版、专业版（18刀）、团队版和企业版。(但是免费版不能使用扩展思维模式)，除了cluade.ai上面可以使用，以下平台也开放了最新Sonnet的访问：以及[Anthropic API](https://docs.anthropic.com/en/docs/about-claude/models)、[Amazon Bedrock](https://aws.amazon.com/bedrock/claude/)和[Google Cloud 的 Vertex AI](https://cloud.google.com/vertex-ai/generative-ai/docs/partner-models/use-claude)上可用

> **PS 需要订阅升级ClaudePro的童鞋参考的详细教程的可以跳转到文末** [(最新教程）Cursor Pro订阅升级开通教程，使用支付宝订阅Cursor Pro Plus](https://littlemagic8.github.io/2024/11/26/how-to-update-cursorPro/)

## Claude Code是什么

Claude Code是一个命令行工具，允许开发者通过终端委托工程任务，显著提升开发效率。

### **Claude Code的使用场景**：

- 该工具在测试驱动开发、调试和大型重构中表现出色，能够显著减少开发时间。
- 未来计划增强工具的可靠性、支持长时间运行的命令，并扩展Claude对自身能力的理解。

### 四步即可安装Claude Code

![img](https://pic2.zhimg.com/v2-bd13e07398434ee860d644dc7ad9e7d3_1440w.jpg)

1. **安装Claude Code** 在终端运行以下命令：

```powershell
npm install -g @anthropic-ai/claude-code
```

**2. 进入项目目录** 使用`cd`命令进入您的项目目录：

```text
cd /path/to/your/project
```

**3. 启动Claude Code** 运行以下命令启动Claude Code：

```text
claude
```

**4. 完成认证** 根据提示完成一次性OAuth认证，您需要在[Anthropic控制台](https://console.anthropic.com/)上拥有有效的计费账户。

## 最后

Claude 3.7总结体验下来

- **Claude 3.7 Sonnet**：Anthropic发布的最新混合推理模型，具备即时响应和深度思考的能力，特别擅长编码和前端开发。**抛开喜欢封号来说，我觉得真的很喜欢cluade,愿意为他扛大旗 为它推广做铜牌销售**
- **Claude Code**：命令行工具，允许开发者通过终端委托工程任务，显著提升开发效率。
- **定价与性能**：模型在所有Claude计划中可用，定价合理，性能在多个基准测试中领先。
- **未来展望**：Claude 3.7 Sonnet和Claude Code标志着AI系统在增强人类能力方面的重要进展。

### CurSor集成了Claude 3.7

目前Cursor以及集成了Claude 3.7，还是Cursor比较友好，大家可以直接在Cursor里面体验，让我们充分发挥以下AI的能力去吧

> **PS：关于Cursor需要升级的可以文末的参考资料**

![img](https://pica.zhimg.com/v2-e931cbaef6f99bf66d3fc0ba9ed7cbd0_1440w.jpg)

## 参考资料：直达☞

API使用教程：[Build with Claude](https://www.anthropic.com/api)

Cursor如何使用订阅升级会员：[(最新教程）Cursor Pro订阅升级开通教程，使用支付宝订阅Cursor Pro Plus](https://littlemagic8.github.io/2024/11/26/how-to-update-cursorPro/)

Claude Pro升级教程：[国内如何使用支付宝注册Claude账号和升级订阅开通Claude Pro](https://littlemagic8.github.io/2024/09/24/use-ClaudePro-model/)

ClaudeCode使用教程：[Write beautiful code, ship powerful products | Claude by Anthropic](https://www.anthropic.com/solutions/coding)

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