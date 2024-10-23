---
layout:     post
title:      Claude HaiKu新模型介绍和Claude Pro新功能使用基础教程【computer use】
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

我们还将推出一项突破性的新功能：**计算机使用**。从今天起，开发人员可以通过 API控制 Claude 以人类的方式使用计算机——查看屏幕、移动光标、单击按钮和输入文本。

## **正文**

![克劳德操作电脑光标的插图](https://www.anthropic.com/_next/image?url=https%3A%2F%2Fwww-cdn.anthropic.com%2Fimages%2F4zrzovbb%2Fwebsite%2Fdb3165778de297272875d36a822f671d8009aaec-2880x1620.png&w=3840&q=75)

# Claude 3.5 Sonnet 计算机使用（测试版）

升级后的 Claude 3.5 Sonnet 模型能够与操纵计算机桌面环境的工具进行交互。

使用计算机是一项测试版功能。请注意，使用计算机会带来与标准 API 功能或聊天界面不同的独特风险。使用计算机与互联网互动时，这些风险会加剧。为了最大限度地降低风险，可以采取以下预防措施：

1. 使用具有最小权限的专用虚拟机或容器，以防止直接的系统攻击或事故。
2. 避免让模型访问敏感数据，例如帐户登录信息，以防止信息盗窃。
3. 将互联网访问限制在域名允许列表中，以减少接触恶意内容。
4. 要求亲自确认可能导致有意义的现实世界后果的决定以及任何需要肯定同意的任务，例如接受 cookie、执行金融交易或同意服务条款。



tips:计算机使用参考实现通过我们的计算机使用参考实现快速开始，其中包括 Web 界面、Docker 容器、示例工具实现和代理循环。(https://github.com/anthropics/anthropic-quickstarts/tree/main/computer-use-demo)

以下是如何使用 Messages API 向 Claude 提供计算机使用工具的示例：python示例

```python
import anthropic

client = anthropic.Anthropic()

response = client.beta.messages.create(
    model="claude-3-5-sonnet-20241022",
    max_tokens=1024,
    tools=[
        {
          "type": "computer_20241022",
          "name": "computer",
          "display_width_px": 1024,
          "display_height_px": 768,
          "display_number": 1,
        },
        {
          "type": "text_editor_20241022",
          "name": "str_replace_editor"
        },
        {
          "type": "bash_20241022",
          "name": "bash"
        }
    ],
    messages=[{"role": "user", "content": "Save a picture of a cat to my desktop."}],
    betas=["computer-use-2024-10-22"],
)
print(response)
```

## 计算机的执行流程

![该图片无替代文字](https://media.licdn.com/dms/image/v2/D4E22AQHvwP7Nlw0XWQ/feedshare-shrink_2048_1536/feedshare-shrink_2048_1536/0/1717362047875?e=2147483647&v=beta&t=IA62sWZ9XoIo1h4KLbg0JvOfZmgm8BiLAIplXpp69Sc)

1. 为 Claude 添加计算机使用工具和用户提示

- 将定义的计算机使用工具添加到您的 API 请求中。
- 包括可能需要这些工具的用户提示，例如“将猫的图片保存到我的桌面”。



2. Claude对操作进行响应决策如何使用工具

- Claude 加载存储的计算机使用工具定义并评估是否有任何工具可以帮助用户的查询。
- 如果是，Claude 会构建一个格式正确的工具使用请求。
- API 响应有一个`stop_reason`，`tool_use`表明 Claude 的意图。



3. 提取工具输入，在计算机上评估工具并返回结果

- 在您的终端，从 Claude 的请求中提取工具名称和输入。
- 在容器或虚拟机上使用该工具。
- `user`使用包含内容块的新消息继续对话`tool_result`。



4. Claude 继续调用计算机使用工具，直到它完成任务

- Claude分析工具结果以确定是否需要使用更多工具或任务是否已完成。
- 如果 Claude 决定它需要另一个工具，它会用另一个工具进行响应`tool_use` `stop_reason`，此时返回步骤 3。
- 否则，它会向用户制作文本响应。

我们将无需用户输入而重复步骤 3 和 4 称为“代理循环” - 即，Claude 使用工具使用请求进行响应，而您的应用程序使用评估该请求的结果来响应 Claude。

## **如何注册Claude账号和升级订阅开通Claude Pro**

**升级订阅开通Claude会员教程**：关于订阅Claude Pro参考[教程](https://littlemagic8.github.io/2024/09/24/use-ClaudePro-model/)

在开通和使用Claude的过程中，如遇到任何问题，欢迎咨询我！aicygg888

**PS:Claude真的好用但是真的太容易封号了！！！如果你需要镜像账号可以使用下面的参考**:[镜像账号](https://littlemagic8.github.io/2024/09/13/GPT-o1-get/)



### 通过提示优化模型性能

以下是有关如何获得最佳质量输出的一些提示：

1. 指定简单、定义明确的任务并为每个步骤提供明确的说明。
2. Claude 有时会在不明确检查结果的情况下假设其操作的结果。为了防止这种情况，你可以使用`After each step, take a screenshot and carefully evaluate if you have achieved the right outcome. Explicitly show your thinking: "I have evaluated step X..." If not correct, try again. Only when you confirm a step was executed correctly should you move on to the next one.`
3. 某些 UI 元素（如下拉列表和滚动条）对于 Claude 来说可能难以通过鼠标移动进行操作。如果您遇到这种情况，请尝试提示模型使用键盘快捷键。
4. 对于可重复的任务或 UI 交互，请在提示中包含成功结果的示例屏幕截图和工具调用。



如果您反复遇到一组明确的问题或提前知道 Claude 需要完成的任务，请使用系统提示为 Claude 提供有关如何成功完成任务的明确提示或说明

