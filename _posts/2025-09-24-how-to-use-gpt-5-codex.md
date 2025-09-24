---
layout:     post
title:      【2025年】GPT-5-Codex来袭！哪些用户能使用GPT-5-Codex？手把手教你如何安装并使用GPT-5-Codex附订阅、ChatGPT Plus代充升级的最新教程，轻松使用GPT5、GPT4o、GPTo3、GPT4.1、GPT4.5版本所有功能！！！
subtitle:   GPT-5-Codex和ChatGPTPlus代充订阅升级
date:       2025-09-24
author:     aicygg888
header-img: img/post-bg-cook.jpg
catalog: true
tags:
    - GPT-5-Codex
---

前段时间的 GPT-5-Codex 更新之后，越来越多的人开始用起来了 OpenAI 的 Codex 了，因为用的人多了，也开始有很多童鞋问我怎样使用 Codex。

今天就来说说如何在(win、macos、Linux)使用Codex，说明在安装使用过程中可能存在的问题及解决方案~

## **一、什么是 Codex ?**

Codex 是 OpenAI 专门针对编程方面工具，它有云端的 Codex Web，也有本地的终端版本 Codex CLI。

**据悉最新的 GPT-5-Codex 模型在大型复杂任务上能够一次独立工作超过 7 小时！（真！牛！马！）**

AI编程有很多种形式的工具，有IDE的、有CLI的、也有云端版的。 比如大家都熟悉的 Cursor 就是 AI IDE 编辑器、**而 Codex 是跟 Claude Code、Gemini CLI 这些都有CLI的。**

**为什么不选择 Claude Code 了？** 因为 Claude Code 最近经常降智、而且 Claude 容易封号（对我们很不友好！！），大多伙伴都是直接使用 Claude Code 镜像的。

而 Codex 封号情况没有那么糟糕，而且 ChatGPT Plus 订阅版比较便宜，几乎人手一个，大家都可以随手试试 Codex 。

## **二、如何安装 Codex ？**

Codex 它可以直接在 ChatGPT 网页上使用，也可以直接在本地安装对应的 Codex CLI，Codex 也可以直接在 VS Code IDE 上安装对应的扩展插件，UI看起来就是跟 Cursor 一样

![img](https://pica.zhimg.com/80/v2-7d5fc3aebb0903f4953d43721d8add07_720w.png?source=ccfced1a)

### **2.1 方式一：在 IDE 上使用 Codex**

**哪些 IDE 工具支持 Codex 扩展插件呢？** 你可以在 VS Code、Cursor、Windsurf 等，搜索对应的 Codex 插件就可以看到官方的Codex。

下面我就以 **VS Code IDE** 为例子教大家怎么安装。

首先，打开你的IDE，在插件市场搜索 Codex ，注意识别是 OpenAI 的标志的 Codex，不然你会安装到其他插件去了。

![img](https://picx.zhimg.com/80/v2-ebd27bd42e8223c15c29723707eafaee_720w.png)

记得安装Codex之前先去更新一下VS code版本哦~

![img](https://pica.zhimg.com/80/v2-aae7b19eab48d9903632223b0fbdde39_720w.png?source=ccfced1a)

安装成功之后，你就可以在你的IDE左上方看到 OpenAI 的图标

![img](https://pic1.zhimg.com/80/v2-394be3a269aa8a7a1397d13579eed0d8_720w.png)

比如你要改什么文件，或者其它想做什么，直接在输入框输入即可~ 另外也可以切换你的模型，平时我都是直接使用 gpt-5-codex (high）

![img](https://pica.zhimg.com/80/v2-65342d6446c5d05091348788f1470285_720w.png)

对于小白来说，你直接在 IDE 安装 Codex 是最方便的了。 而且操作都是有 GUI 界面，降低了上手难度。

### **2.2 方式二：在终端使用 Codex CLI**

Codex CLI 是一个编码代理，您可以从终端本地运行，并且可以在计算机上读取、修改和运行代码。

如果你是 Mac用户，直接安装 Codex CLI 就行，随时都可以调起你的 Codex 进行 AI 编程。

**因为目前的 Codex CLI 支持在 macOS 和 Linux。Windows 仍处于实验阶段，建议在 WSL 中运行。**

你直接在 Windows 安装的话，会出现一些乱码甚至各种奇怪的麻烦，处理这些问题估计一整天就要过去了。

**Codex CLI 两种安装方式：npm 和 Homebrew。**

（1）使用 npm 的话, 需要先安装一下 NodeJS 环境。

如果系统是 Ubuntu / Debian 的 Linux用户，可以使用下面的命令安装Node.js：

```
curl -fsSL https://deb.nodesource.com/setup_22.x | sudo bash -
sudo apt-get install -y nodejs
node --version
npm --version
```

如果系统是 MacOS 的用户，可以用下面的命令安装Node.js：

```bash
sudo xcode-select --install
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
sudo brew install node
node --version
```

确保你的 npm 和 Nodejs可以使用时，就可以通过以下命令安装 Codex CLI：

```bash
npm install -g @openai/codex
```

（2）使用 Homebrew 安装 Codex：

```bash
brew install codex
```

**两种方式，选择其中之一就行，我是已经有NodeJS环境，所以就用第一种方式进行安装了。**

安装之后，创建一个目录，然后在目录下开启你的终端，执行 codex 就可以唤醒 Codex CLI 

![img](https://picx.zhimg.com/80/v2-e4ec120860a8b29e328695f2c5709ef7_720w.png)

## **三、Codex CLI 的使用分享**

在使用 Codex CLI，大家可能会出现跟我一样的疑惑或者问题，都可以参考以下方式解决。

### **3.1 如何设置 Codex 以中文回复**

这个你可以直接在终端告诉它一直使用中文回复，但是重启之后可能就失效了。所以你可以通过 Codex 特殊的记忆文件：AGENTS.md。

你可以在当前目录，执行 /init 它就会在当前工作空间生成。 但是不符合我们的场景，我们需要全局的，那么可以跟我这样子操作。

在 ~/.codex/ 下 创建一个 AGENTS.md 文件，然后输入 **“Always respond in Chinese-simplified”** 在里面。

你也可以复制以下指令，在你的终端执行即可：

```bash
mkdir -p ~/.codex && printf 'Always respond in Chinese-simplified\n' > ~/.codex/AGENTS.md
```

### **3.2 如何切换和查看当前模型**

执行 /model 就可以切换和查看自己正在使用的模型，优先推荐 GPT-5-Codex (high)。

```bash
/model
```

### **3.3 本地如何启动登录授权 Codex CLI**

本地的话，大家一定要记得开启全局路由，也就是你魔法的TUN模式！最近太多人使用 Codex 了，OpenAI 的算力负载也提高了很多，所以可能会检测一些滥用的用户进行封号。

避免这种情况，建议在你的魔法（TZ）工具上，开启对应的全局 TUN 模式。

![img](https://picx.zhimg.com/80/v2-aa0651c930ecaa82f1c2e5e38766a3a5_720w.png)

## **四、Codex CLI 哪些用户可以使用？**

Codex 目前只能给订阅了 GPT 会员的用户才能使用，如果你不知道这么升级自己的 GPT Plus 的话，可以使用下方的一键升级：

使用我**开发的GPT一键升级系统**，几分钟内完成，三步搞定~ (需要订阅其它AI服务可以戳我VX：aicygg888)

>  **GPT 一键升级系统**：[OpenAI GPT代充系统](https://littlemagic8.github.io/gptplus/) ：https://littlemagic8.github.io/gptplus/ (使用浏览器打开)

![img](https://pic1.zhimg.com/80/v2-07d554dd68abfacd60d0e4d0665ca7e6_720w.png)

**不知道怎么使用的话，看代充系统上图文或者视频教程即可，很简单 2 分钟就搞定 GPT 的升级~**

## **五、Windows 上安装 WSL 使用 Codex CLI**

### **5.1 安装WSL，必须满足以下要求：**

- Windows 11 或 Windows 10 21H2以上，专业版/工作站版/企业版（非家庭版，需支持Hyper-V）
- CPU 需支持且已在 BIOS/UEFI 中启用虚拟化

### **（1）按照以下步骤安装WSL：**

安装之前需要打开虚拟化，否则过程会出现未知的错误。

打开路径：控制面板 -> 程序与功能 -> 打开或关闭 Windows 功能 启动以下功能：

- Virtual Machine Platform（虚拟机平台）
- Windows Subsystem for Linux Support（WSL）

**下载和安装对应版本的 WSL，** 选择您的系统版本，复制到浏览器进行下载 WSL 安装包:

- 64-Bit WSL-2.5.9.0 [推荐]

```bash
https://vip.123pan.cn/1831946356/links/wsl.2.5.9.0.x64.msi
```

- ARM64 WSL-2.5.9.0

```bash
https://vip.123pan.cn/1831946356/links/wsl.2.5.9.0.arm64.msi
```

- ARM64_MicrosoftStore WSL-2.5.9.0

```bash
https://vip.123pan.cn/1831946356/links/Microsoft.WSL_2.5.9.0_x64_ARM64.msixbundle
```

**你也可以不用上面的安装包，直接访问 GitHub 安装最新的版本：**

> https://github.com/microsoft/WSL/releases

### **（2）安装虚拟机：**

安装完WSL之后，你可以在微软应用商店中安装最新的Ubuntu 24.04 LTS 或者 通过以下命令安装：

```bash
wsl --install -d Ubuntu-24.04
```

**如果执行后遇到包错的情况，无法链接之类的，是因为网络问题，可以开一下魔法，或者修改一下 github 的host本地dns的解析IP。（也可以问AI）**

你也可通过 wsl -l -o 命令选择其他系统版本。

安装完 **Ubuntu** 之后，你可以在**终端（或PowerShell）**输入wsl访问安装的操作系统：

- **首次用需要设置用户名和密码：**

>  如果您通过开始菜单的应用访问一次，直接关闭窗口而不输入用户名和密码，下次访问将使用root用户

- Windows将安装的操作系统虚拟机视作一个应用，如Ubuntu 24.04 LTS 会出现在你的开始菜单

### **（3）Windows 的 Codex CLI 安装**

安装完Ubuntu之后，你只需在CMD或者终端工具上，运行wsl就可以进入。

```bash
wsl
```

接着，就可以在wsl下面，进行运行和部署 Codex CLI。 **安装步骤跟上面的 Ubuntu/Linux 👆 系统 安装的流程一致。**

大家还需要Grok、Gemini、Claude、Cursor等AI工具均可代充，可以直接找我微信：aicygg888

1. 出Midjourney 30刀 质保/不质保

2. 出ChatGPT pro200刀质保

3. 低价出3个月90天plus现货，带RT

4. 出Grok 30刀/300刀 质保/不质保

5. 出GPT Plus 20刀 质保/不质保

6. 低价出 gemini ultra  veo3  质保/不质保，25000积分

**低价代打以下Ai产品，全部比官网价格低 (无质保)**
1️⃣gptplus成品/链接代充
2️⃣pika10/35成品/代充
3️⃣flowith20成品/代充
4️⃣manus39代充
5️⃣ naturalreader21刀
6️⃣runway35刀
7️⃣minimax39刀
8️⃣ bolt.new 25刀
9️⃣lovart19刀
🔟 krea 35刀
🎉ponde30刀

## **小提示：如果你想使用更多AI产品，可以联系V: aicygg888**

> **如果不想开通信用卡可以参考：无需开通信用卡完成ChatGPT订阅教程：ChatGPTplus独享账号的自助订阅升级（无需开通visa、master等支付卡片、无痛解决chatGPTplus支付问题）**
>
> > *ChatGPTplus独享账号升级充值自助平台：*[*https://littlemagic8.github.io/gptplus/*](https://littlemagic8.github.io/gptplus/) *（网站下方有购买卡密和使用教程参考）*
>
> **PS:如果你需要开通自己的ChatGPT Plus、Claude Pro的个人独享账号可以参考教程：**[**使用支付方式订阅开通ChatGPT Plus、Claude Pro教程**](https://littlemagic8.github.io/2024/09/04/update-ChatGPT-Plus/) （https://littlemagic8.github.io/2024/09/04/update-ChatGPT-Plus/） *PS：国内直接使用chatGPT/Claude镜像账号可以通过两种方式获取：*

方式一：通过教程自行购买：

（遇到问题，联系微信：aicygg888 登录地址：https://chatshare.biz/ (复制到浏览器打开）用购买成功后的账号密码登录 自动购买地址，买完即可用 购买地址：https://littlemagic8.github.io/buychat/ ）

> - **ChatGPT** **Plus独享账号教程**：https://littlemagic8.github.io/2025/07/17/chatgptplus-auto-system/
> - **Claude** **Pro订阅指南**：https://littlemagic8.github.io/2024/12/09/ChatGPT-and-Cluade/
> - **镜像账号使用说明**：https://littlemagic8.github.io/2025/07/17/chatgptplus-chatshare/

不想自己注册账号，可以用方式二

> *方式二：添加微信购买 微信：***aicygg888** *(备注镜像账号哦)*

欢迎加微信

![img](https://picx.zhimg.com/80/v2-46f7cfd62d1e94381388ab08b0fea3af_720w.png)

公众号也可以哦

![img](https://pic1.zhimg.com/80/v2-4e622b64238b20948a02e0c988ca5704_720w.png)





 