---
layout:     post
title:      nano-banana如何使用保姆级教程，五大应用实例供你参考， -助你代订阅gemini-advanced，轻松使用nano-banana模型附自助充值chatgptplus
subtitle:   nano-banana使用保姆级教程
date:       2025-09-01
author:     aicygg888
header-img: img/post-bg-cook.jpg
catalog: true
tags:
    - nano-banana
---

最近被香蕉刷屏了，google悄咪咪干大事~

Google的Gemini Nano-Banana（正式名Gemini 2.5 Flash Image）横空出世，一夜之间碾压全球图像编辑模型，成为竞技场的number one！

![img](https://picx.zhimg.com/80/v2-3bf959238a7dd36e3dd996f16f12c85e_720w.png)

这个“纳米香蕉”听说不光出图飞快，而且在人物一致性、融合多图、智能编辑更是一绝，简直是创作者的神器。

无论是产品摄影师、社交达人还是设计师，都在疯狂安利！

今天，我来手把手教你如何上手，还附上5大应用场景的提示词+实例演示。读完这篇，助力你创作出更多爆款内容！（文末有福利，记得点赞+关注哦~）

## Gemini Nano-Banana是什么？

Gemini Nano-Banana是Google DeepMind推出的AI图像生成与编辑模型，基于Gemini 2.5 Flash架构，专攻高效、低成本的创意编辑。

它能融合多张图片、保持人物一致性、用自然语言精准修改（如“模糊背景”或“换衣服”），甚至利用“世界知识”生成语义准确的图像。

**为什么叫“Nano-Banana”？**

这是Google的内部昵称，源自测试时的匿名代号，现在已正式集成到Gemini app和API中。

接下来和小编一起来体验使用一下纳米香蕉，有官方使用地址传送门和详细使用流程。

## **超详细教程：如何使用Gemini Nano-Banana（含地址+实际流程）**

Gemini Nano-Banana可以通过多种方式访问：

1、Google AI Studio

2、Gemini

3、API集成（开发者）（也可以直接使用我们接入API的现成的镜像站）**接下来也是用镜像站进行演示**

>  PS：需要镜像站使用图文教程参考：https://littlemagic8.github.io/2025/07/17/chatgptplus-chatshare/

4、第三方平台如Imogen app、Bylo.ai、Freepik

tips: 免费版有水印，付费（Gemini Advanced）无限使用。

> **ps: 需要代充订阅Gemini Advanced可以找我（aicygg888）**

### **步骤1：访问地址并登录**

- Google AI Studio：[aistudio.google.com](https://aistudio.google.com/)
- Gemini: https://gemini.google.com/。
- 第三方选项：镜像(chatshare.biz)。
- 开发者，可用API密钥（从[ai.google.dev](https://ai.google.dev/)获取）。

### **步骤2：使用nano-banana**

- 在AI Studio首页，点击“New prompt”或“Start chatting”。
- 选择模型：切换到“Gemini 2.5 Flash Image”（或搜索“nano-banana”）。

![img](https://picx.zhimg.com/80/v2-189934b91deee9d0bc31c80cb161ce88_720w.png)

- 如果用Gemini ：进入图像编辑模式（点击相机图标）。

![img](https://pic1.zhimg.com/80/v2-5dd9102e708a8d85819a1b3647cc7069_720w.png)

镜像站入口，选择“备用plus入口”->"画图系列模型"

![img](https://picx.zhimg.com/80/v2-7f58bea81e9fec461f2f811b4a6bca37_720w.png)

### **步骤3：上传图像并输入提示**

类似下图

![img](https://picx.zhimg.com/80/v2-4027b8fdd6916c7c4823619ba0b682d4_720w.png)

### **步骤4：优化**

- 优化Tips：提示要具体（如“保持面部一致性”）；
- 多图融合时，指定“融合A图的沙发到B图的客厅”；
- 免费版限额小，升级Gemini Advanced无限用 需要升级可以找我：aicygg888。

示例：在镜像站（镜像站要抽卡，我就用Google AI Studio试试吧~）中上传自拍照，提示“把我放到太空，穿宇航服”，输出后迭代“添加地球背景” 一张科幻头像就诞生了！

![img](https://pic1.zhimg.com/80/v2-b72bd66383657e0382fb7ff831b76caf_720w.png)

![img](https://pic1.zhimg.com/80/v2-77331ab0a10391a45953288f8c313a86_720w.png)



![img](https://pic1.zhimg.com/80/v2-6b428cde4c7af1486de1253c57e057c3_720w.png)

![img](https://picx.zhimg.com/80/v2-d0cc34d099db759be068ec701ce270f9_720w.png)

![img](https://picx.zhimg.com/80/v2-cf3b6dd8fe10a21a00091cd1135418e7_720w.png)



开发者模式：用API集成？安装SDK（pip install google-generativeai），代码示例：

```
from google import genai
from PIL import Image
from io import BytesIO

client = genai.Client(api_key='YOUR_API_KEY')
prompt = "Create a nano banana dish in a fancy restaurant"
response = client.models.generate_content(model="gemini-2.5-flash-image-preview", contents=[prompt])
image = Image.open(BytesIO(response.candidates[0].content.parts[0].inline_data.data))
image.save("output.png")
```

地址：[ai.google.dev/gemini-api/docs/image-generation](https://ai.google.dev/gemini-api/docs/image-generation)。

接下来，来看5大应用场景（社交达人、商家、设计师、教学、游戏）等方面进行展示，每个附提示词+实例！

## **5大应用场景：提示词+实例演示，解锁无限创意**

Gemini Nano-Banana的强大在于多场景适应。下面我选了5个热门领域，每个给出实用提示词和实例（基于真实输出模拟）。这些都能在AI Studio或app中直接试！

### **1. 时尚与自拍编辑（适合社交达人）**

- **提示词**："Change my outfit to a medieval Indian princess saree with flowers in hair, deep center parting. 你穿着纱丽，站在田野中，面部细节完美保留 Keep my face realistic and consistent."

![img](https://picx.zhimg.com/80/v2-caf38ba7a7aca8e501bbcaed7397efb4_720w.png)

### **2. 产品摄影与电商（适合商家）**

- **提示词**："A model is posing and leaning against a pink bmw. She is wearing the following items, the scene is against a light grey background. The green alien is a keychain and it's attached to the pink handbag. The model also has a pink parrot on her shoulder. There is a pug sitting next to her wearing a pink collar and gold headphones."

![img](https://pica.zhimg.com/80/v2-789f98fb66435d52fa473aefe374f6f5_720w.png)

### **3. 室内设计可视化（适合设计师）**

- **提示词**："empty room photo. Paint walls blue, add bookshelf, coffee table, and sofa from this color palette. Keep lighting natural."

![img](https://pic1.zhimg.com/80/v2-43b7f3b4b37bcdd72e984ff526b7559f_720w.png)

### **4. 教育与图表生成（适合老师/学生）**

- **提示词**："绘制一幅展示公鸡的3D立体剖面设计图，以高度还原的方式精细呈现其内部结构。每个零部件被拆解并有序排列，各部分均配有清晰中文标注，注明结构名称与功能说明，整体布局兼具专业性与视觉逻辑性，呈现出清晰、整洁且极具真实性的解析示意图。"

![img](https://picx.zhimg.com/80/v2-bb1fe9d90381c601049d4ffa61405acc_720w.png)

### **5. 游戏与头像设计（适合游戏爱好者）**

- **提示词**："Generate avatar from this photo: Make me a space explorer with helmet, add alien pet on shoulder. Multiple angles for consistency."

![img](https://picx.zhimg.com/80/v2-49f74bc2f0340509402a11e1d57c9ef7_720w.png)



## **结语：Nano-Banana，让你的创意“香蕉”起来！**

**这个教学用户的3D模型用来教学一个小白是不现实的，所以对于教学方面暂时不可用的感觉，对于商家和设计师来讲应该还挺不错的，后续简单的ps完全不用了，用嘴就行，包括证件照，完全不在话下~**

![img](https://picx.zhimg.com/80/v2-7e6ba6ac28908a2ccbf01dcbae284782_720w.png)

就这种感觉~

Gemini Nano-Banana 有抽卡的几率，有条件的还是订阅Gemini advanced会员吧！

有疑问评论区见，一起脑洞大开~ 🚀🍌



因为wildcard跑路，很多童鞋想要订阅使用ChatGPTplus可以参考下面教程

#  升级 ChatGPT 详细步骤 （推荐✨）

有客户使用礼品卡的方式进行升级，礼品卡对网络和 Apple ID 还是比较严格的，**个人如果操作不当，可能会被风控到自己的 Apple ID 之类的**。

如果喜欢折腾的还是可以尝试一下的礼品卡，不喜欢花这个时间的话，可以通过下面这种方式进行升级 GPT PLUS。**（已经使用了5个月，稳定、靠谱的代升级方式！）**

下面的原理也是跟礼品卡的一样，通过20刀的礼品卡一次性充值 GPT的方式，前提都是需要你的 GPT 已经到期了，**处于 free 的账号状态**。

> **GPT升级系统：** *https://littlemagic8.github.io/gptplus/* （使用浏览器打开）

进入之后，可以查看对应的视频教程，然后再回来进行操作升级。

**整个升级流程大概如下（2分钟就可以完成升级）

![img](https://pic1.zhimg.com/80/v2-b706045d6bd0b1c2dafa91f22dd3bcdf_720w.png)



> **GPT升级系统：** *https://littlemagic8.github.io/gptplus/* （使用浏览器打开）

# 其它代充服务

大家还需要Grok、Gemini、Claude、Cursor等AI工具均可代充，可以直接找我微信：aicygg888



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



官方宣传提示词：https://developers.googleblog.com/en/how-to-prompt-gemini-2-5-flash-image-generation-for-the-best-results/

