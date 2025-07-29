---
layout:     post
title:      AI Cursor Cline Chatbox OpenAI API 使用教程？
subtitle:   Cursor Cline Chatbox OpenAI
date:       2025-04-30
author:     aicygg888
header-img: img/post-bg-cook.jpg
catalog: true
tags:
    - API
---

## **前言**


官网：https://littlemagic8.github.io/pay/



# 介绍

API 随心用的底层通过对接由[OpenAI官方](https://platform.openai.com/docs/api-reference/chat/create) 和 [Azure OpenAI](https://azure.microsoft.com/zh-cn/products/ai-services/openai-service) 提供的 **OpenAI模型、**由[Amazon Bedrock](https://aws.amazon.com/cn/bedrock/)提供的**Anthropic Claude模型** 从而实现用户无需注册 OpenAI 和 Anthropic 账号绑卡即可任意网络直连GPT-4/Claude 3.5。

用户在API 随心用管理界面创建专属于自己的API Key

[![img](https://downloads.intercomcdn.com/i/o/sjswlknd/1261755056/3795a8b1653b480e8072e730247f/image.png?expires=1745994600&signature=d379218e6ffdf8cbdc09fbd72b0a307cb7b4b0a73bf31771fcf84408e1eb703d&req=dSIhF857mIFaX%2FMW1HO4zXP3tFlGJvJMpLibZJkt8YLn7dz8ixgCjLdfa4U%2B%0AfARspAx2O9BCRlvvOLE%3D%0A)](https://downloads.intercomcdn.com/i/o/sjswlknd/1261755056/3795a8b1653b480e8072e730247f/image.png?expires=1745994600&signature=d379218e6ffdf8cbdc09fbd72b0a307cb7b4b0a73bf31771fcf84408e1eb703d&req=dSIhF857mIFaX%2FMW1HO4zXP3tFlGJvJMpLibZJkt8YLn7dz8ixgCjLdfa4U%2B fARspAx2O9BCRlvvOLE%3D )

然后即可通过`[https://api.gptsapi.net`](https://api.gptsapi.net`/) 域名下的接口访问不同功能和价位的AI模型：

教程定价表可能出现未实时更新的情况，具体价格以网站api定价tab展示的定价表为准

 

# Cursor 接入 API

## 1. 在 setting 的 models 里面点击 Override OpenAI Base URL

[![img](https://downloads.intercomcdn.com/i/o/sjswlknd/1369450422/788d38e5ee869e458079392fe795/20250207-155910.jpeg?expires=1745994600&signature=71866feab03dfa4a956fcf5d1bba97174c8ae343d3a6dd910689e3e1b598fd78&req=dSMhH817nYVdW%2FMW1HO4zcUoTFYswNU9haJuLKd0%2FtFnGI0kDbE1CJitxHlN%0AVsa1YIdy%2B9fJBAm6t0c%3D%0A)](https://downloads.intercomcdn.com/i/o/sjswlknd/1369450422/788d38e5ee869e458079392fe795/20250207-155910.jpeg?expires=1745994600&signature=71866feab03dfa4a956fcf5d1bba97174c8ae343d3a6dd910689e3e1b598fd78&req=dSMhH817nYVdW%2FMW1HO4zcUoTFYswNU9haJuLKd0%2FtFnGI0kDbE1CJitxHlN Vsa1YIdy%2B9fJBAm6t0c%3D )

##  2. 填入 2233  base URL https://api.gptsapi.net/v1 和 2233 的 API key

OpenAI 模型就可以直接调用了

##  3. 调用 Claude

同样在 OpenAI API key 模式下，不要切换到 Anthropic API key。
点击 add model，可以增加以下模型（用 wild 替换模型中的 claude ，opus 和 haiku 同理）:
wild-3-5-sonnet-20240620
wild-3-5-sonnet-20241022
wild-3-7-sonnet-20250219	

 

即可正常调用 claude sonnet 模型。
​

[![img](https://downloads.intercomcdn.com/i/o/sjswlknd/1369447429/a6c02b6cf5e2618cd66f2c6b1458/output.jpg?expires=1745994600&signature=3f0ba73f33b3295e219a97789f1dd2c0028e137bf150ae3a16d7cc438ad5bb50&req=dSMhH816moVdUPMW1HO4zXYjlUJObp1%2FFwMHmit3B54iqADUi4vB5nW4pcxY%0AHFGFXXWzlWaeG1H7VMk%3D%0A)](https://downloads.intercomcdn.com/i/o/sjswlknd/1369447429/a6c02b6cf5e2618cd66f2c6b1458/output.jpg?expires=1745994600&signature=3f0ba73f33b3295e219a97789f1dd2c0028e137bf150ae3a16d7cc438ad5bb50&req=dSMhH816moVdUPMW1HO4zXYjlUJObp1%2FFwMHmit3B54iqADUi4vB5nW4pcxY HFGFXXWzlWaeG1H7VMk%3D )

#   Cline 接入 API

## 1. 点击 cline 头像，在 Settings 中，选择 API Provider 为 OpenAI Compatible

 

## 2. 填入 2233  base URL https://api.gptsapi.net/v1 和 2233 的 API key

OpenAI 模型就可以直接调用了

 

## 3. 调用 Claude

同样在 OpenAI Compatible 模式下， 输入 model id 即可正常调用：
claude-3-5-sonnet-20241022

claude-3-5-sonnet-20240620

claude-3-7-sonnet-20250219	

 

 

[![img](https://downloads.intercomcdn.com/i/o/sjswlknd/1369456538/44607853a85c5d19a865d1ce6bdf/image.png?expires=1745994600&signature=8e6da398831335985372e44546509cc3eac5e453410fc1af33c9c7e3953ae47d&req=dSMhH817m4RcUfMW1HO4zeOPWwQlaxGHNCMYAIvp9tbJzyGm7YobOgYOU2z9%0AM6GDg8%2BRz313%2FCE85f8%3D%0A)](https://downloads.intercomcdn.com/i/o/sjswlknd/1369456538/44607853a85c5d19a865d1ce6bdf/image.png?expires=1745994600&signature=8e6da398831335985372e44546509cc3eac5e453410fc1af33c9c7e3953ae47d&req=dSMhH817m4RcUfMW1HO4zeOPWwQlaxGHNCMYAIvp9tbJzyGm7YobOgYOU2z9 M6GDg8%2BRz313%2FCE85f8%3D )

 

#   Chat 客户端使用 API

Chat客户端，旨在提高与大型语言模型（如ChatGPT、Claude）的交互效率。它们提供本地数据存储、多模型支持、图像生成、高级Prompt、美观的UI界面等各种功能，适用于个人和团队使用。这些客户端支持多种操作系统，包括Windows、Mac、Linux，甚至提供Web、iOS和Android版本，以满足不同用户的需求。

下面介绍开源Chat客户端如何配置使用 API：

 

 我们推荐 chatbox 和 [chatx](https://apps.apple.com/us/app/chatx-ai-chat-client-top/id6446304087) 两个客户端，设置基本大同小异。

 

## Cherry Studio 

在设置里的 model provider，点击最底部的 add provider
​

[![img](https://downloads.intercomcdn.com/i/o/sjswlknd/1404853891/63eb82bb27421c8a28fe378c7209/Screenshot+2025-03-03+at+23_11_57.png?expires=1745994600&signature=e020f1904c8a5d2153bfdf7d667d8deb19e0fc4643dfa6b9ce3faca3e98b4986&req=dSQnEsF7nolWWPMW1HO4zaZDjt6FRk0D%2FLucMFkcrbyFbPAsnzaZTchWtM%2Fi%0Apb2%2FQbq%2BtuEDLDuLE9Q%3D%0A)](https://downloads.intercomcdn.com/i/o/sjswlknd/1404853891/63eb82bb27421c8a28fe378c7209/Screenshot+2025-03-03+at+23_11_57.png?expires=1745994600&signature=e020f1904c8a5d2153bfdf7d667d8deb19e0fc4643dfa6b9ce3faca3e98b4986&req=dSQnEsF7nolWWPMW1HO4zaZDjt6FRk0D%2FLucMFkcrbyFbPAsnzaZTchWtM%2Fi pb2%2FQbq%2BtuEDLDuLE9Q%3D )

 然后填写名称，注意 type 一定要填写 openai（用  claude 模型也是）要选这个 type；

[![img](https://downloads.intercomcdn.com/i/o/sjswlknd/1404852320/21a096256de87aaa5b9dfbb97930/Screenshot+2025-02-25+at+16_02_37.png?expires=1745994600&signature=f87f0b0c3cd8258eddd7ea17122149f06648639edcf936dbf146a4a1dcbd53d8&req=dSQnEsF7n4JdWfMW1HO4zXxuJ2RsDgz4HVUUEUgky%2F0qyic9MoCvvH8lIDE6%0AOgfz8jcQM7SnnOtVAow%3D%0A)](https://downloads.intercomcdn.com/i/o/sjswlknd/1404852320/21a096256de87aaa5b9dfbb97930/Screenshot+2025-02-25+at+16_02_37.png?expires=1745994600&signature=f87f0b0c3cd8258eddd7ea17122149f06648639edcf936dbf146a4a1dcbd53d8&req=dSQnEsF7n4JdWfMW1HO4zXxuJ2RsDgz4HVUUEUgky%2F0qyic9MoCvvH8lIDE6 Ogfz8jcQM7SnnOtVAow%3D )

然后依次填写我们的 api key 和 api host，记得不要加 /v1，只填写 [https://api.gptsapi.net](https://api.gptsapi.net/) 即可。

[![img](https://downloads.intercomcdn.com/i/o/sjswlknd/1404858871/dff5245b78b023ac1ee81373bcc0/20250303-231420.png?expires=1745994600&signature=364ca533427d2a35882c20bd80fbbcfb2a0b0fb1e7628d47011aff42699838af&req=dSQnEsF7lYlYWPMW1HO4zYUQBN%2FZsW8KZGWFN5cQLY54bJ7sBIgQR9PY%2BWCL%0AXWkyaOhPpIIZNW1Yyi4%3D%0A)](https://downloads.intercomcdn.com/i/o/sjswlknd/1404858871/dff5245b78b023ac1ee81373bcc0/20250303-231420.png?expires=1745994600&signature=364ca533427d2a35882c20bd80fbbcfb2a0b0fb1e7628d47011aff42699838af&req=dSQnEsF7lYlYWPMW1HO4zYUQBN%2FZsW8KZGWFN5cQLY54bJ7sBIgQR9PY%2BWCL XWkyaOhPpIIZNW1Yyi4%3D )

然后添加模型名称即可，gpt 和 claude 的模型都支持。

 

## Chatbox

官网：https://chatboxai.app/zh#
​

设置自定义Claude模型服务商

[![img](https://downloads.intercomcdn.com/i/o/sjswlknd/1261769555/21b6ce669b7f57fa6c4f50551d34/image.png?expires=1745994600&signature=c38cadacfbacd718bb4bb0817929b7ef4f9954197c6e72399448fc128c6ced7b&req=dSIhF854lIRaXPMW1HO4zR4SoFHE47fAiUh2Jjzhj%2F7yv0G9UcJ2BTHnuyMf%0AdUSLJqTMOtjjsK06lNw%3D%0A)](https://downloads.intercomcdn.com/i/o/sjswlknd/1261769555/21b6ce669b7f57fa6c4f50551d34/image.png?expires=1745994600&signature=c38cadacfbacd718bb4bb0817929b7ef4f9954197c6e72399448fc128c6ced7b&req=dSIhF854lIRaXPMW1HO4zR4SoFHE47fAiUh2Jjzhj%2F7yv0G9UcJ2BTHnuyMf dUSLJqTMOtjjsK06lNw%3D )

设置自定义OpenAI模型服务商

[![img](https://downloads.intercomcdn.com/i/o/sjswlknd/1261771369/01c339e86c43005b1ec0eed954f0/image.png?expires=1745994600&signature=c87ac3c34d96bc334d23f67dd3af60f912e96b210827d67c60d708d492dec1f6&req=dSIhF855nIJZUPMW1HO4zdMLe2GxZNElZDcijKHUrcZF9d9AS4F2BX7Y35qS%0AeNbb0v8uTRe2Wsui%2Ba4%3D%0A)](https://downloads.intercomcdn.com/i/o/sjswlknd/1261771369/01c339e86c43005b1ec0eed954f0/image.png?expires=1745994600&signature=c87ac3c34d96bc334d23f67dd3af60f912e96b210827d67c60d708d492dec1f6&req=dSIhF855nIJZUPMW1HO4zdMLe2GxZNElZDcijKHUrcZF9d9AS4F2BX7Y35qS eNbb0v8uTRe2Wsui%2Ba4%3D )

保存设置后即可进行聊天沟通

[![img](https://wildcard-b0518949163b.intercom-attachments-7.com/i/o/1003881127/1d6e3151bc25861d0a2c997c/asynccode?expires=1745994600&signature=44181e80892c526fe36a2dd6f98217b3f1930cdd0c683d1c492af116bbec21f7&req=dSAnFcF2nIBdXvMW1HO4zRIQiTbOYDV2zQY%2Bpr%2FrmA%2F3kXz0HXJvqDZOzd5p%0AIxJ8%2BeP32wsebqN4qYo%3D%0A)](https://wildcard-b0518949163b.intercom-attachments-7.com/i/o/1003881127/1d6e3151bc25861d0a2c997c/asynccode?expires=1745994600&signature=44181e80892c526fe36a2dd6f98217b3f1930cdd0c683d1c492af116bbec21f7&req=dSAnFcF2nIBdXvMW1HO4zRIQiTbOYDV2zQY%2Bpr%2FrmA%2F3kXz0HXJvqDZOzd5p IxJ8%2BeP32wsebqN4qYo%3D )

 

# 接口调用 API

## 身份验证

API 随心用 与 OpenAI API 和 Anthropic API 一样皆使用 API Key进行身份验证，并兼容两者的请求方式：

所有 API 请求都应在 HTTP 请求头中包含您的 API Key，使用`Authorization` 或者`x-api-key` 作为Header Key。

curl请求示例如下：（$API_KEY替换为用户创建的专属API Key）

```
curl https://api.gptsapi.net/v1/models \-H "Authorization: Bearer $API_KEY"
curl https://api.gptsapi.net/v1/models \-H "x-api-key: $API_KEY"
```

## 聊天接口（Chat）

### /v1/chat/completions

OpenAI聊天接口，接口定义参考https://platform.openai.com/docs/api-reference/chat/create

 

请求示例
Python 代码示例：
​

```
from openai import OpenAI

# 创建客户端时指定自定义的 base URL
client = OpenAI(
    api_key="",# 您在 2233 创建的 key
    base_url="https://api.gptsapi.net/v1"  # 我们提供的 url
)

# 发送请求
response = client.chat.completions.create(
    model="gpt-3.5-turbo",
    messages=[
        {
            "role": "user",
            "content": "Hello!"
        }
    ]
)

# 打印返回结果
print(response.choices[0].message.content)
```

curl请求示例如下：（$API_KEY替换为用户创建的专属API Key）

```
curl https://api.gptsapi.net/v1/chat/completions \-H "Content-Type: application/json" \-H "Authorization: Bearer $API_KEY" \-d '{ "model": "gpt-3.5-turbo-0125", "messages": [ { "role": "user", "content": "Hello!" } ] }'
```

 

### /v1/messages

Anthropic聊天接口，接口定义参考https://docs.anthropic.com/claude/reference/messages_post

支持模型列表

- claude-3-sonnet-20240229
- claude-3-haiku-20240307
- claude-3-opus-20240229	
- claude-3-5-sonnet-20240620	
- claude-3-5-sonnet-20241022	
- claude-3-5-haiku-20241022	

 

请求示例

有两种请求方式，一种是 OpenAI 格式的，一种是 Claude 格式的，我们均支持。
Python 代码示例：
​

```
from openai import OpenAI

# 创建客户端时指定自定义的 base URL
client = OpenAI(
    api_key="",# 您在 2233 创建的 key
    base_url="https://api.gptsapi.net/v1"  # 我们提供的 url
)

# 发送请求
response = client.chat.completions.create(
    model="claude-3-5-sonnet-20241022", #填写claude模型名称即可
    messages=[
        {
            "role": "user",
            "content": "Hello!"
        }
    ]
)

# 打印返回结果
print(response.choices[0].message.content)
import anthropic

def chat_with_claude(api_key, message, base_url=None):
    client = anthropic.Anthropic(
        api_key=api_key,
        base_url=base_url
    )
    
    try:
        response = client.messages.create(
            model="claude-3-5-sonnet-20241022",
            max_tokens=1000,
            messages=[{"role": "user", "content": message}]
        )
        return response.content
    except Exception as e:
        print(f"错误: {str(e)}")
        raise

if __name__ == "__main__":
    api_key = ""  #在 2233 创建的 api key
    base_url = "https://api.gptsapi.net"
    print(chat_with_claude(api_key, "你好", base_url))
```


curl请求示例如下：（$API_KEY替换为用户创建的专属API Key）

```
curl https://api.gptsapi.net/v1/messages \--header "x-api-key: $API_KEY" \--header "anthropic-version: 2023-06-01" \--header "content-type: application/json" \--data \ '{ "model": "claude-3-haiku-20240307", "max_tokens": 1024, "messages": [ {"role": "user", "content": "Hello, world"} ] }'
```

## OpenAI 嵌入接口（Embeddings）

### /v1/messages

OpenAI嵌入接口，接口定义参考https://platform.openai.com/docs/api-reference/embeddings/create

支持模型列表

- text-embedding-ada-002
- text-embedding-3-small
- text-embedding-3-large

请求示例

curl请求示例如下：（$API_KEY替换为用户创建的专属API Key）

```
curl https://api.gptsapi.net/v1/embeddings \-H "Content-Type: application/json" \-H "Authorization: Bearer $API_KEY" \-d '{ "input": "The food was delicious and the waiter...", "model": "text-embedding-ada-002", "encoding_format": "float" }'
```

## OpenAI 图像接口（Images）

### /v1/images/generations

OpenAI创建图像接口，接口定义参考https://platform.openai.com/docs/api-reference/images/create

支持模型列表

- dall-e-3
- dall-e-2

请求示例

curl请求示例如下：（$API_KEY替换为用户创建的专属API Key）

```
curl https://api.gptsapi.net/v1/images/generations \-H "Content-Type: application/json" \-H "Authorization: Bearer $API_KEY" \-d '{ "model": "dall-e-3", "prompt": "A cute baby sea otter", "n": 1, "size": "1024x1024" }'
```

## 音频接口（Audio）

### /v1/audio/speech

OpenAI创建语音接口，接口定义参考https://platform.openai.com/docs/api-reference/audio/createSpeech

支持模型列表

- tts-1
- tts-1-hd

请求示例

curl请求示例如下：（$API_KEY替换为用户创建的专属API Key）

```
curl https://api.gptsapi.net/v1/audio/speech \-H "Content-Type: application/json" \-H "Auth
```



## 小提示：如果你想使用更多AI产品，可以联系V: aicygg888

> **PS:如果你需要开通自己的ChatGPT Plus、Claude Pro的个人独享账号可以参考教程：**[**使用支付方式订阅开通ChatGPT Plus、Claude Pro教程**](https://littlemagic8.github.io/2024/09/04/update-ChatGPT-Plus/) （https://littlemagic8.github.io/2024/09/04/update-ChatGPT-Plus/）
>
> *PS：国内直接使用chatGPT/Claude镜像账号可以通过两种方式获取：*

方式一：通过教程自行购买：

（遇到问题，联系微信：aicygg888
登录地址：https://chatshare.biz/ (复制到浏览器打开）用购买成功后的账号密码登录
自动购买地址，买完即可用 购买地址：https://fk.yfk66.top//links/3C9CE3BA ）

> *1、*[**镜像账号购买**](https://littlemagic8.github.io/2024/12/09/ChatGPT-and-Cluade/)：[https://littlemagic8.github.io/2024/12/09/ChatGPT-and-Cluade/](https://littlemagic8.github.io/2024/12/09/ChatGPT-and-Cluade/ ) 
>
> *2、*[**镜像账号购买参考**](https://littlemagic8.github.io/2025/04/10/how-use-share-AI-model/) https://littlemagic8.github.io/2025/04/10/how-use-share-AI-model/

不想自己注册账号，可以用方式二

> *方式二：添加微信购买 微信：***aicygg888** *(备注镜像账号哦)*

欢迎加微信

![img](https://picx.zhimg.com/80/v2-46f7cfd62d1e94381388ab08b0fea3af_720w.png)

公众号也可以哦

![img](https://pic1.zhimg.com/80/v2-4e622b64238b20948a02e0c988ca5704_720w.png)





