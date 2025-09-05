---
layout:     post
title:      谷歌nano-banana手把手超详细使用教程，教你如何使用gemini-advanced
subtitle:   nano-banana使用保姆级教程
date:       2025-09-03
author:     aicygg888
header-img: img/post-bg-cook.jpg
catalog: true
tags:
    - nano-banana
---

最近被香蕉刷屏了，google悄咪咪干大事~

Google的Gemini Nano-Banana（正式名Gemini 2.5 Flash Image）横空出世，一夜之间碾压全球图像编辑模型，成为竞技场的number one！

![img](https://picx.zhimg.com/80/v2-3bf959238a7dd36e3dd996f16f12c85e_720w.png)

nano-banana听说在人物一致性、融合多图很不错，那我们今天就来看看到底怎么样。

今天，我来手把手教你如何上手，还附上5大应用场景的提示词+实例演示。读完这篇，助力你创作出更多爆款内容！（文末有福利，记得点赞+关注哦~）

## Gemini Nano-Banana是什么？

Gemini Nano-Banana是Google DeepMind推出的AI图像生成与编辑模型，基于Gemini 2.5 Flash架构，专攻高效、低成本的创意编辑。

它能融合多张图片、保持人物一致性、用自然语言精准修改（如“模糊背景”或“换衣服”），甚至利用“世界知识”生成语义准确的图像。

**为什么叫“Nano-Banana”？**

这是Google的内部昵称，源自测试时的匿名代号，现在已正式集成到Gemini app和API中。

接下来和小编一起来体验使用一下纳米香蕉，有官方使用地址传送门和详细使用流程。

## 如何使用Gemini Nano-Banana

Gemini Nano-Banana可以通过多种方式访问：

1、Google AI Studio

2、Gemini

3、API方式（也可以直接使用我们接入了Nano Banana API的现成chatshare.biz镜像站，使用图文教程参考 https://littlemagic8.github.io/2025/07/17/chatgptplus-chatshare/ ）

4、第三方平台如Imogen app、Bylo.ai、Freepik

tips: 免费版有水印，付费（Gemini Advanced）无限使用。

> **ps: 需要代充订阅Gemini Advanced可以找我（aicygg888）**

### 官网地址

- Google AI Studio：[aistudio.google.com](https://aistudio.google.com/)
- Gemini: https://gemini.google.com/。
- 第三方选项：镜像(chatshare.biz)。
- 开发者，可用API密钥（从[ai.google.dev](https://ai.google.dev/)获取）。

### **三个姿势去使用nano-banana**

**方式一：AI Studio**

- 在**AI Studio**首页，点击“New prompt”或“Start chatting”。
- 选择模型：切换到“Nano-Banana“。

![img](https://picx.zhimg.com/80/v2-189934b91deee9d0bc31c80cb161ce88_720w.png)

**方式二：Gemini**

- 进入图像编辑模式,如下图所示

![img](https://pic1.zhimg.com/80/v2-5dd9102e708a8d85819a1b3647cc7069_720w.png)

**方式三：chatshre.biz 镜像站**

镜像站入口，选择“备用plus入口”->"画图系列模型"

> ps: 需要镜像站可以参考本教程：https://littlemagic8.github.io/2025/07/17/chatgptplus-chatshare/

![img](https://picx.zhimg.com/80/v2-7f58bea81e9fec461f2f811b4a6bca37_720w.png)



示例：在镜像站（镜像站要抽卡，我就用Google AI Studio试试吧~）中上传自拍照，提示“把我放到太空，穿宇航服”，输出后迭代“添加地球背景” 一张科幻头像就诞生了！

![img](https://pic1.zhimg.com/80/v2-b72bd66383657e0382fb7ff831b76caf_720w.png)

![img](https://pic1.zhimg.com/80/v2-77331ab0a10391a45953288f8c313a86_720w.png)



![img](https://pic1.zhimg.com/80/v2-6b428cde4c7af1486de1253c57e057c3_720w.png)

![img](https://picx.zhimg.com/80/v2-d0cc34d099db759be068ec701ce270f9_720w.png)

![img](https://picx.zhimg.com/80/v2-cf3b6dd8fe10a21a00091cd1135418e7_720w.png)



方式四：开发者模式

代码示例：

```python
from google import genai
from PIL import Image
from io import BytesIO

client = genai.Client(api_key='YOUR_API_KEY')
prompt = "Create a nano banana dish in a fancy restaurant"
response = client.models.generate_content(model="gemini-2.5-flash-image-preview", contents=[prompt])
image = Image.open(BytesIO(response.candidates[0].content.parts[0].inline_data.data))
image.save("output.png")
```

开发者地址传送门：[ai.google.dev/gemini-api/docs/image-generation](https://ai.google.dev/gemini-api/docs/image-generation)。



## 实例体验

接下来，来看5大应用场景（社交达人、商家、设计师、教学、游戏）等方面进行展示，每个附提示词+实例！

Gemini Nano-Banana的强大在于多场景适应。下面我选了5个热门领域，每个给出实用提示词和实例（基于真实输出模拟）。这些都能在AI Studio或app中直接试！

### **场景1. 时尚与自拍编辑**

- **提示词**："Change my outfit to a medieval Indian princess saree with flowers in hair, deep center parting. 你穿着纱丽，站在田野中，面部细节完美保留 Keep my face realistic and consistent."

![img](https://picx.zhimg.com/80/v2-caf38ba7a7aca8e501bbcaed7397efb4_720w.png)

### **场景2. 产品摄影与电商**

- **提示词**："A model is posing and leaning against a pink bmw. She is wearing the following items, the scene is against a light grey background. The green alien is a keychain and it's attached to the pink handbag. The model also has a pink parrot on her shoulder. There is a pug sitting next to her wearing a pink collar and gold headphones."

![img](https://pica.zhimg.com/80/v2-789f98fb66435d52fa473aefe374f6f5_720w.png)

### **场景3. 室内设计可视化**

- **提示词**："empty room photo. Paint walls blue, add bookshelf, coffee table, and sofa from this color palette. Keep lighting natural."

![img](https://pic1.zhimg.com/80/v2-43b7f3b4b37bcdd72e984ff526b7559f_720w.png)

### **场景4. 教育与图表生成**

- **提示词**："绘制一幅展示公鸡的3D立体剖面设计图，以高度还原的方式精细呈现其内部结构。每个零部件被拆解并有序排列，各部分均配有清晰中文标注，注明结构名称与功能说明，整体布局兼具专业性与视觉逻辑性，呈现出清晰、整洁且极具真实性的解析示意图。"

![img](https://picx.zhimg.com/80/v2-bb1fe9d90381c601049d4ffa61405acc_720w.png)

### **场景5. 游戏与头像设计**

- **提示词**："Generate avatar from this photo: Make me a space explorer with helmet, add alien pet on shoulder. Multiple angles for consistency."

![img](https://picx.zhimg.com/80/v2-49f74bc2f0340509402a11e1d57c9ef7_720w.png)



## END：Nano-Banana，让你的创意“NB”起来！

**这个教学用户的3D模型用来教学一个小白是不现实的，所以对于教学方面暂时不可用的感觉，对于商家和设计师来讲应该还挺不错的，毕竟人物一致性真的很不错！！！**

后续简单的ps完全不用了，用嘴就行，包括证件照，完全不在话下~

![img](https://picx.zhimg.com/80/v2-7e6ba6ac28908a2ccbf01dcbae284782_720w.png)

就这种感觉~

Gemini Nano-Banana 有抽卡的几率，有条件的还是订阅Gemini advanced会员吧！**需要订阅gemini 会员可以找我：aicygg888** 

有疑问评论区见，一起脑洞大开~ 🚀🍌



因为wildcard跑路，很多童鞋想要订阅使用ChatGPTplus可以参考下面教程


整个升级流程大概如下（2分钟就可以完成升级）

![img](https://pic1.zhimg.com/80/v2-b706045d6bd0b1c2dafa91f22dd3bcdf_720w.png)



> **GPT升级系统：** *https://littlemagic8.github.io/gptplus/* （使用浏览器打开）

# 其它代充服务

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



官方宣传提示词：https://developers.googleblog.com/en/how-to-prompt-gemini-2-5-flash-image-generation-for-the-best-results/

 