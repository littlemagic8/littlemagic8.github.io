---
layout:     post
title:      Grok发布了Grok Studio 和 Workspaces两个强大的功能。该如何使用？如何使用Grok3 API？
subtitle:   Grok Studio、Workspaces
date:       2025-04-27
author:     aicygg888
header-img: img/post-bg-cook.jpg
catalog: true
tags:
    - Grok3
---

## **前言**


![img](https://pic1.zhimg.com/80/v2-1fcaa64239f3a5cc5ee1b96321ffc477_720w.png)



## 最近Grok又更新了几个功能：Grok Studio 和 Workspaces。

其中 Grok Studio 主要功能包括：

1. 代码执行：在预览标签中运行 HTML 片段、Python、JavaScript 等。
2. Google Drive 集成：附加并处理 Docs、Sheets、Slides等文件。
3. 协作工作空间：一起编辑和润色内容。
4. 适用于文档撰写（论文、报告）、代码开发（网站、应用）、数据分析（表格处理）及创意项目（游戏、艺术展示）

![img](https://picx.zhimg.com/80/v2-09d7670a5b492f68e59da3f5352210b1_720w.png)

也就是Grok Studio 是一个协作环境，可以生成文档、代码、报告，甚至浏览器游戏等，同时它提供实时预览（类似genspark、manus），写完代码就能立刻运行查看效果，支持多种编程语言，还能与Google Drive集成，直接处理Drive上的文件。

Grok Studio 提供分屏界面，左侧为 Grok 聊天窗口，右侧为编辑区，适合实时协作。它支持多种任务，如编写代码、生成文档或开发简单游戏，类似 OpenAI 的 Canvas，但免费访问是其优势。

**目前Grok Studio功能已经对免费和付费用户都开放，极大提升了创作效率。**

你可以直接上传一份csv数据，就可以让Grok直接生成一份报告。

![img](https://picx.zhimg.com/80/v2-91377c50ee0c66b689ace231fb49206a_720w.png)

而Workspace（工作空间）功能，工作空间可以帮助你在一个地方组织文件和对话，并且**可以设定自定义指令**。使用工作空间可以跟踪假期规划、学习资料、工作流程和自定义个性。

![img](https://picx.zhimg.com/80/v2-02801b5c078624946511ad1739143535_720w.png)

Workspaces 主要解决了普通聊天模式中上下文丢失的问题。

通过将对话和文件绑定到特定 Workspace，Grok 能够更好地保持长期项目的上下文，即使在多次会话中也能记住之前的进展。

支持用户在 Workspace 给每个工作空间改名字，同时支持给workspace下达你的指令约束它，除此之外使用 Grok 的其他模型，如 DeepSearch、Deeper Search 和 Think Mode，以增强任务处理能力。

![img](https://pic1.zhimg.com/80/v2-3b8591ddda0d80c5a712c2a8a3dfd85a_720w.png)

## **Grok、Claude、ChatGPT 之间的对比**

**Grok Workspaces：**

- 优点：免费用户可用性高，限制较少，支持实时搜索和多种工具整合，界面简洁，适合个人用户或需要快速任务处理的小型团队。
- 缺点：第三方整合较弱，自定义选项不如 ChatGPT 灵活，文档深度分析能力稍逊于 Claude。
- 适用场景：个人项目管理、实时信息检索、快速任务处理（如旅行规划、学习笔记整理）。

**ChatGPT Projects：**

- 优点：插件生态丰富，自定义能力强，适合需要复杂工作流或多媒体任务（图像生成、长文本创作）的用户。
- 缺点：免费用户功能受限，部分高级功能需要订阅 Plus。
- 适用场景：内容创作、营销、需要第三方工具整合的复杂项目。

**Claude Projects：**

- 优点：文档分析和团队协作能力强，Artifacts 功能提升了长文本和代码的管理效率，适合知识密集型任务。
- 缺点：免费用户消息限制严格，缺乏图像生成等功能，第三方整合不如 ChatGPT。
- 适用场景：学术研究、团队协作、复杂文档处理。

## Grok3 API发布了

在发布了Grok Studio 和 Workspaces，Grok还上线了 Grok-3-mini API！其中Grok 3 Mini 的性能远超推理模型，成本却降低了 5 倍，重新定义了经济高效的智能。Grok 3 是全球最强大的非推理模型，在法律、金融和医疗保健等需要现实世界知识的任务中表现出色。如下图所示

![img](https://picx.zhimg.com/80/v2-20a3f0a18a120b666ff780882b0de53e_720w.png)

![img](https://pic1.zhimg.com/80/v2-a1bea0de147116cacae33f539b6075a3_720w.png)



**使用下面代码即可使用Grok3 API 模型**

```
from openai import OpenAI
    
client = OpenAI(
  api_key=XAI_API_KEY,
  base_url="https://api.x.ai/v1",
)

completion = client.chat.completions.create(
  model="grok-3-beta",
  messages=[
    {"role": "user", "content": "What is the meaning of life?"}
  ]
)
```

## **海外支付解决方案**

相信很多伙伴在订阅ChatGPT Plus 或者 Grok、Claude、OpenRouter 时，都遇到银行卡绑定失败的情况。这是因为它们需要国际的visa、master卡才能进行订阅支付。

**很多人没有这类型的卡，那么你可以申请一张虚拟Master卡解决。**

比如，我常用的是这个Master虚拟卡，使用了2年，到期我还会续，真的觉得不错~

> Master虚拟卡：https://littlemagic8.github.io/pay/

![img](https://pic1.zhimg.com/80/v2-91371e46b90e80f6b56d52fe4b222b60_720w.png)

需要订阅什么服务，点击对应的服务，使用支付宝充值对应的余额之后，根据里面的教程进行订阅就行。

比如，我需要订阅OpenRouter Pro，点击之后就是类似下面这样子，有属于你对应的卡片信息和账单地址。

![img](https://pic1.zhimg.com/80/v2-98f91eeca2d7ce37551a7f2a6590f580_720w.png)



对小白和新手非常友好，有问题也可以直接咨询客服。

如果Grok3次数免费不够用，或者需要提高次数的话，可以通过订阅 X（原推特）的Premium 小蓝v服务，然后再通过 X 登录 Grok.com。可以提高Grok3的次数。

关于如何订阅Grok可以参考：[(2025最新)如何使用Grok3，如何订阅X Premuim+ P+高级会员，教你每月白嫖 150 美元的免费Grok3 API 积分](https://littlemagic8.github.io/2025/02/19/how-use-Gork3_API/)

## Gork3 分析425政治局会议

> 根据2025年4月25号中共中央政治局召开的会议，清晰概述后续的工作力度在哪。分析哪些方便的股票可能比较有希望涨，分析黄金的走势，包括关键行动、目标以及这些政策的利弊。涵盖政治和经济背景，包括各方反应和市场趋势。请把这些内容渲染成网页内容供传阅

```
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>2025年4月25日中共中央政治局会议经济分析报告</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 20px;
            background-color: #f4f4f4;
        }
        .container {
            max-width: 800px;
            margin: auto;
            background: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        h1, h2, h3 {
            color: #333;
        }
        h1 {
            text-align: center;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }
        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: left;
        }
        th {
            background-color: #f2f2f2;
        }
        ul, ol {
            margin: 10px 0;
            padding-left: 20px;
        }
        a {
            color: #0066cc;
            text-decoration: none;
        }
        a:hover {
            text-decoration: underline;
        }
        .citation {
            font-size: 0.9em;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>2025年4月25日中共中央政治局会议经济分析报告</h1>
        
        <h2>会议概述</h2>
        <p>2025年4月25日，中共中央政治局召开会议，分析当前经济形势并部署经济工作，由习近平总书记主持 (<a href="https://www.gov.cn/yaowen/liebiao/202504/content_7020941.htm">政治局会议</a>)。会议指出，中国经济呈现向好态势，社会信心持续提振，但复苏基础需进一步巩固，外部冲击影响加大。政策目标是通过稳中求进、深化改革和扩大开放，实现高质量发展和社会稳定。</p>

        <h2>后续工作力度重点</h2>
        <p>会议明确了以下重点工作领域，以推动经济持续向好：</p>
        <table>
            <tr>
                <th>领域</th>
                <th>具体措施</th>
            </tr>
            <tr>
                <td>宏观经济政策</td>
                <td>实施更积极的财政政策和适度宽松的货币政策，加快发行专项债券，适时降息，保持流动性充裕。</td>
            </tr>
            <tr>
                <td>消费与收入</td>
                <td>提高中低收入群体收入，发展服务消费，扩大“两新”政策，增强消费拉动作用。</td>
            </tr>
            <tr>
                <td>企业支持</td>
                <td>支持困难企业，培育新质生产力，发展新兴支柱产业，推进关键技术突破。</td>
            </tr>
            <tr>
                <td>改革与开放</td>
                <td>深化改革，建设全国统一大市场，扩大服务领域试点，支持企业走出去。</td>
            </tr>
            <tr>
                <td>风险防范</td>
                <td>化解地方政府债务，处理房地产问题，维护资本市场稳定。</td>
            </tr>
        </table>

        <h2>股票市场分析</h2>
        <p>会议的政策信号可能对以下板块的股票产生积极影响，但投资者需关注市场波动和政策执行的不确定性：</p>
        <ul>
            <li><strong>科技板块</strong>：会议提出推出债券市场“科技板”和加速“人工智能+”行动，人工智能、半导体和新能源等高科技企业可能受益。例如，科创板相关股票可能因政策支持而表现强劲。</li>
            <li><strong>基建与建筑</strong>：加快专项债券发行和“两新一重”（新型基础设施、新型城镇化、重大工程）建设将为基建和建筑行业提供资金支持，相关企业如中国建筑可能迎来增长机会。</li>
            <li><strong>消费板块</strong>：提高中低收入群体收入和发展服务消费的政策可能提振消费品和服务行业，零售和旅游相关股票可能表现良好。</li>
            <li><strong>房地产</strong>：城市更新、城中村改造和新房地产模式的推进可能为房地产开发商和建筑材料企业带来机会，但需警惕市场调整风险。</li>
        </ul>
        <p>尽管政策利好可能推动市场上涨，投资者应注意外部经济环境和政策落地效果的不确定性。市场分析表明，A股在政策刺激下可能短期内表现积极，但长期表现取决于全球经济和国内执行情况。</p>

        <h2>黄金走势分析</h2>
        <p>黄金作为避险资产，其价格受货币政策和全球经济不确定性影响。会议提及的适度宽松货币政策和降息措施可能降低实际利率，利好黄金价格。此外，外部冲击（如地缘政治或贸易紧张）增加可能进一步推高黄金需求。根据市场预测 (<a href="https://longforecast.cn/%E9%87%91%E4%BB%B7%E6%A0%BC%E8%B5%B0%E5%8A%BF%E9%A2%84%E6%B5%8B-2017-2018-2019">黄金价格预测</a>)，2025年4月25日黄金价格预计为3459美元/盎司，范围在3286至3632美元之间。长期来看，高盛等机构预测2025年底金价可能达到3000美元/盎司 (<a href="https://www.xhby.net/content/s6773ce80e4b0595c185fc41d.html">2025年黄金展望</a>)，受全球央行购金和投资需求推动。然而，短期内金价可能因市场调整或利率预期变化而波动。截至2025年4月27日，黄金期货价格为3298.40美元/盎司，较前日下跌1.50%，但年度涨幅达41.26% (<a href="https://cn.investing.com/commodities/gold">黄金期货行情</a>)，显示整体上涨趋势。</p>

        <h2>政策的关键行动与目标</h2>
        <p>会议提出以下关键行动和目标，以应对经济挑战并推动高质量发展：</p>
        <ul>
            <li><strong>行动</strong>：
                <ul>
                    <li>实施积极财政政策，加速专项债券发行，增加基础设施投资。</li>
                    <li>适度宽松货币政策，适时降息和降准，保持流动性充裕。</li>
                    <li>推出新结构性货币工具和政策性金融工具，支持创新、消费和贸易。</li>
                    <li>提高中低收入群体收入，发展服务消费，清除消费限制。</li>
                    <li>支持企业发展，培育新质生产力，推进“科技板”和“AI+”行动。</li>
                    <li>深化改革，建设全国统一大市场，扩大高水平对外开放。</li>
                    <li>防范风险，化解地方政府债务，稳定房地产和资本市场。</li>
                </ul>
            </li>
            <li><strong>目标</strong>：
                <ul>
                    <li>实现经济稳定增长，巩固复苏基础。</li>
                    <li>稳定就业，增强社会信心。</li>
                    <li>推动高质量发展，培育新兴产业。</li>
                    <li>维护社会稳定，应对外部不确定性。</li>
                </ul>
            </li>
        </ul>

        <h2>政策的利弊分析</h2>
        <p>这些政策在刺激经济和稳定市场的同时，也带来潜在风险。以下是利弊的详细分析：</p>
        <table>
            <tr>
                <th>方面</th>
                <th>优势</th>
                <th>劣势</th>
            </tr>
            <tr>
                <td>经济增长</td>
                <td>财政和货币刺激可促进投资和消费，创造就业机会。</td>
                <td>过度刺激可能导致通胀压力或资产泡沫。</td>
            </tr>
            <tr>
                <td>科技创新</td>
                <td>支持人工智能和新兴产业可增强中国在全球科技领域的竞争力。</td>
                <td>高投入可能需要较长时间见效，短期回报不确定。</td>
            </tr>
            <tr>
                <td>消费提振</td>
                <td>提高收入和消费能力可增强内需，减少对出口依赖。</td>
                <td>消费政策可能加剧财政压力，需平衡分配公平性。</td>
            </tr>
            <tr>
                <td>资本市场</td>
                <td>稳定市场政策可吸引投资，提升信心。</td>
                <td>市场干预可能导致资源配置扭曲，影响长期效率。</td>
            </tr>
            <tr>
                <td>债务与风险</td>
                <td>化解债务和房地产风险有助于长期稳定。</td>
                <td>短期内可能增加政府债务负担，需谨慎管理。</td>
            </tr>
        </table>

        <h2>政治与经济背景</h2>
        <p>政治局会议是中国最高决策机构制定的经济政策方向，反映了中央对国内外形势的判断。当前，中国经济在2024年实现平稳增长，高质量发展稳步推进，但面临外部冲击（如贸易紧张和地缘政治风险）以及国内复苏基础不稳的挑战。会议强调以高质量发展的确定性应对外部不确定性，显示出中国在复杂全球环境中坚持自主发展的决心。国内政策制定者通过加强党对经济工作的领导，确保政策协调和执行效率。</p>

        <h2>各方反应</h2>
        <p>国内分析师对会议政策普遍持乐观态度，认为积极的财政和货币政策将提振市场信心并刺激经济增长。例如，财经媒体指出，政策重点如“保企业、稳就业”将为资本市场注入活力 (<a href="https://wap.stockstar.com/detail/IG2025042500025392">热点追踪</a>)。国际上，部分观察家可能因中美贸易紧张或地缘政治因素对政策效果持谨慎看法。例如，瑞银等机构对中国股市持中性观点，强调地缘政治风险 (<a href="https://cn.investing.com/indices/shanghai-composite">上证指数行情</a>)。整体而言，市场对政策反应积极，但长期效果取决于全球经济环境和政策执行情况。</p>

        <h2>市场趋势</h2>
        <p>股票市场预计对政策刺激措施反应积极，尤其是在科技、基建、消费和房地产板块。A股市场可能在政策利好下短期内上涨，但需警惕外部经济波动和政策落地效果的不确定性。黄金市场在全球不确定性下持续受到关注，2025年价格预计保持上涨趋势，但短期波动可能因市场调整而发生。投资者应密切关注宏观经济数据和政策执行进展，以制定投资策略。</p>

        <h2>结论</h2>
        <p>2025年4月25日政治局会议为中国经济指明了方向，通过积极的财政和货币政策、支持科技创新和消费、深化改革以及防范风险，旨在实现高质量发展和经济稳定。科技、基建、消费和房地产板块的股票可能因政策支持而表现良好，黄金价格预计继续上涨，但投资者需注意短期波动和政策执行风险。这些政策在刺激经济的同时，也需平衡通胀、债务和市场效率等挑战，为中国经济在复杂全球环境中稳健发展奠定基础。</p>

        <div class="citation">
            <h3>关键引用</h3>
            <ul>
                <li><a href="https://www.gov.cn/yaowen/liebiao/202504/content_7020941.htm">中共中央政治局4月25日会议经济形势分析</a></li>
                <li><a href="https://longforecast.cn/%E9%87%91%E4%BB%B7%E6%A0%BC%E8%B5%B0%E5%8A%BF%E9%A2%84%E6%B5%8B-2017-2018-2019">2025年黄金价格走势预测</a></li>
                <li><a href="https://cn.investing.com/commodities/gold">黄金期货实时行情与走势分析</a></li>
                <li><a href="https://www.xhby.net/content/s6773ce80e4b0595c185fc41d.html">2025年黄金市场展望与价格预测</a></li>
                <li><a href="https://wap.stockstar.com/detail/IG2025042500025392">4月政治局会议对股市影响热点追踪</a></li>
                <li><a href="https://cn.investing.com/indices/shanghai-composite">上证指数实时行情与市场分析</a></li>
            </ul>
        </div>
    </div>
</body>
</html>
```



## 小提示：如果你想使用更多AI产品，可以联系V: aicygg888

> **PS:如果你需要开通自己的ChatGPT Plus、Claude Pro的个人独享账号可以参考教程：**[**使用支付方式订阅开通ChatGPT Plus、Claude Pro教程**](https://littlemagic8.github.io/2024/09/04/update-ChatGPT-Plus/) （https://littlemagic8.github.io/2024/09/04/update-ChatGPT-Plus/）
>
> *PS：国内直接使用chatGPT/Claude镜像账号可以通过两种方式获取：*

方式一：通过教程自行购买：

（遇到问题，联系微信：aicygg888
登录地址：https://chatshare.biz/ (复制到浏览器打开）用购买成功后的账号密码登录
自动购买地址，买完即可用 购买地址：https://fk.i6ls.com//links/3C9CE3BA ）

> *1、*[**镜像账号购买**](https://littlemagic8.github.io/2024/12/09/ChatGPT-and-Cluade/)：[https://littlemagic8.github.io/2024/12/09/ChatGPT-and-Cluade/](https://littlemagic8.github.io/2024/12/09/ChatGPT-and-Cluade/ ) 
>
> *2、*[**镜像账号购买参考**](https://littlemagic8.github.io/2025/04/10/how-use-share-AI-model/) https://littlemagic8.github.io/2025/04/10/how-use-share-AI-model/

不想自己注册账号，可以用方式二

> *方式二：添加微信购买 微信：***aicygg888** *(备注镜像账号哦)*

欢迎加微信

![img](https://picx.zhimg.com/80/v2-46f7cfd62d1e94381388ab08b0fea3af_720w.png)

公众号也可以哦

![img](https://pic1.zhimg.com/80/v2-4e622b64238b20948a02e0c988ca5704_720w.png)





