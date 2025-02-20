---
layout:     post
title:      WildCard API 使用教程
subtitle:   WildCard API 使用教程
date:       2024-12-26
author:     aicygg888
header-img: img/post-bg-cook.jpg
catalog: true
tags:
    - API
---



# 介绍

WildCard API 的底层通过对接由[OpenAI官方](https://platform.openai.com/docs/api-reference/chat/create) 和 [Azure OpenAI](https://azure.microsoft.com/zh-cn/products/ai-services/openai-service) 提供的 **OpenAI模型、**由[Amazon Bedrock](https://aws.amazon.com/cn/bedrock/)提供的**Anthropic Claude模型** 从而实现用户无需注册 OpenAI 和 Anthropic 账号绑卡即可任意网络直连GPT-4/Claude 3。

用户在WildCard API 管理界面创建专属于WildCard的API Key

[![img](https://wildcard-b0518949163b.intercom-attachments-7.com/i/o/1003881036/428a2965321cd3c8614b2ed4/asynccode?expires=1718854200&signature=91416741195100080e1e2477fd547eb710c57918fdfd1b9fde1c69ce6e78ec48)](https://wildcard-b0518949163b.intercom-attachments-7.com/i/o/1003881036/428a2965321cd3c8614b2ed4/asynccode?expires=1718854200&signature=91416741195100080e1e2477fd547eb710c57918fdfd1b9fde1c69ce6e78ec48)

然后即可通过`[https://api.gptsapi.net`](https://api.gptsapi.net`/) 域名下的接口访问不同功能和价位的AI模型：

| 产品          | 模型                     | Input              | Output             |
| ------------- | ------------------------ | ------------------ | ------------------ |
| Claude        | claude-3-opus-20240229   | $15.00 / 1M tokens | $75.00 / 1M tokens |
|               | claude-3-sonnet-20240229 | $3.00 / 1M tokens  | $15.00 / 1M tokens |
|               | claude-3-haiku-20240307  | $0.25 / 1M tokens  | $1.25 / 1M tokens  |
| GPT-4o        | gpt-4o-2024-05-13        | $5.00 / 1M tokens  | $15.00 / 1M tokens |
| GPT-4 Turbo   | gpt-4-0125-preview       | $10.00 / 1M tokens | $30.00 / 1M tokens |
|               | gpt-4-1106-preview       | $10.00 / 1M tokens | $30.00 / 1M tokens |
|               | gpt-4-vision-preview     | $10.00 / 1M tokens | $30.00 / 1M tokens |
|               | gpt-4-turbo-preview      | $10.00 / 1M tokens | $30.00 / 1M tokens |
| GPT-4         | gpt-4                    | $30.00 / 1M tokens | $60.00 / 1M tokens |
|               | gpt-4-0613               | $30.00 / 1M tokens | $60.00 / 1M tokens |
|               | gpt-4-0314               | $30.00 / 1M tokens | $60.00 / 1M tokens |
|               | gpt-4-32k                | $60.00 / 1M tokens | $120.0 / 1M tokens |
|               | gpt-4-32k-0314           | $60.00 / 1M tokens | $120.0 / 1M tokens |
|               | gpt-4-32k-0613           | $60.00 / 1M tokens | $120.0 / 1M tokens |
| GPT-3.5 Turbo | gpt-3.5-turbo            | $1.50 / 1M tokens  | $2.00 / 1M tokens  |
|               | gpt-3.5-turbo-16k        | $3.00 / 1M tokens  | $4.00 / 1M tokens  |
|               | gpt-3.5-turbo-0125       | $0.50 / 1M tokens  | 1.50 / 1M tokens   |
|               | gpt-3.5-turbo-instruct   | $1.50 / 1M tokens  | $2.00 / 1M tokens  |

# Chat 客户端使用WildCard API

Chat客户端，旨在提高与大型语言模型（如ChatGPT、Claude）的交互效率。它们提供本地数据存储、多模型支持、图像生成、高级Prompt、美观的UI界面等各种功能，适用于个人和团队使用。这些客户端支持多种操作系统，包括Windows、Mac、Linux，甚至提供Web、iOS和Android版本，以满足不同用户的需求。

下面介绍二个成熟的开源Chat客户端如何配置使用WildCard API：

 

## NextChat

开源项目地址：https://github.com/ChatGPTNextWeb/ChatGPT-Next-Web

设置自定义模型服务商

[![img](https://wildcard-b0518949163b.intercom-attachments-7.com/i/o/1003881049/684a567f3199b2b5c10e6c66/asynccode?expires=1718854200&signature=482756562d024572806ba8676618c2695171fa52b933fd47af0c7a02a3473b5b)](https://wildcard-b0518949163b.intercom-attachments-7.com/i/o/1003881049/684a567f3199b2b5c10e6c66/asynccode?expires=1718854200&signature=482756562d024572806ba8676618c2695171fa52b933fd47af0c7a02a3473b5b)

切换AI模型，NextChat暂不支持Claude模型

[![img](https://wildcard-b0518949163b.intercom-attachments-7.com/i/o/1003881064/448fd9cdcee3a93df815d4fd/asynccode?expires=1718854200&signature=043ae2b1c8cfa8c3f5be81c35fdf81bda304ff5cf0856b17afd0939ce6177ef0)](https://wildcard-b0518949163b.intercom-attachments-7.com/i/o/1003881064/448fd9cdcee3a93df815d4fd/asynccode?expires=1718854200&signature=043ae2b1c8cfa8c3f5be81c35fdf81bda304ff5cf0856b17afd0939ce6177ef0)

设置完成即可进行聊天沟通

[![img](https://wildcard-b0518949163b.intercom-attachments-7.com/i/o/1003881077/8d135156f6dcf2c2156cc944/asynccode?expires=1718854200&signature=25f83faf28138d27d7cb029386a8d69a1bf4295acdf5422b3c44a3d6f1a701ed)](https://wildcard-b0518949163b.intercom-attachments-7.com/i/o/1003881077/8d135156f6dcf2c2156cc944/asynccode?expires=1718854200&signature=25f83faf28138d27d7cb029386a8d69a1bf4295acdf5422b3c44a3d6f1a701ed)

 

## Chatbox

开源项目地址：https://github.com/Bin-Huang/chatbox

设置自定义Claude模型服务商

[![img](https://wildcard-b0518949163b.intercom-attachments-7.com/i/o/1003881101/da02a529522124c127c2deda/asynccode?expires=1718854200&signature=ab9c593cae61c9752b086d097bb857fa4c861de124e83e22856f8b255092ad48)](https://wildcard-b0518949163b.intercom-attachments-7.com/i/o/1003881101/da02a529522124c127c2deda/asynccode?expires=1718854200&signature=ab9c593cae61c9752b086d097bb857fa4c861de124e83e22856f8b255092ad48)

设置自定义OpenAI模型服务商

[![img](https://wildcard-b0518949163b.intercom-attachments-7.com/i/o/1003881109/1b33e9b374ef6ff89ec0dcac/asynccode?expires=1718854200&signature=5bbd90614578258474368828ca16ff843c30ecc399bd37e8ad9a910e0db07a12)](https://wildcard-b0518949163b.intercom-attachments-7.com/i/o/1003881109/1b33e9b374ef6ff89ec0dcac/asynccode?expires=1718854200&signature=5bbd90614578258474368828ca16ff843c30ecc399bd37e8ad9a910e0db07a12)

保存设置后即可进行聊天沟通

[![img](https://wildcard-b0518949163b.intercom-attachments-7.com/i/o/1003881127/1d6e3151bc25861d0a2c997c/asynccode?expires=1718854200&signature=6ccdf9e35f02a0ca0fad21f723f2cb746fb03a79d76bcc5801a4588a5d2d8944)](https://wildcard-b0518949163b.intercom-attachments-7.com/i/o/1003881127/1d6e3151bc25861d0a2c997c/asynccode?expires=1718854200&signature=6ccdf9e35f02a0ca0fad21f723f2cb746fb03a79d76bcc5801a4588a5d2d8944)

 

# 接口调用WildCard API

## 身份验证

WildCard API 与 OpenAI API 和 Anthropic API 一样皆使用 API Key进行身份验证，并兼容两者的请求方式：

所有 API 请求都应在 HTTP 请求头中包含您的 API Key，使用`Authorization` 或者`x-api-key` 作为Header Key。

curl请求示例如下：（$API_KEY替换为WildCard创建的专属API Key）

```
curl https://api.gptsapi.net/v1/models \-H "Authorization: Bearer $API_KEY"
curl https://api.gptsapi.net/v1/models \-H "x-api-key: $API_KEY"
```

## 聊天接口（Chat）

### /v1/chat/completions

OpenAI聊天接口，接口定义参考https://platform.openai.com/docs/api-reference/chat/create

支持模型列表

- gpt-3.5-turbo
- gpt-3.5-turbo-16k
- gpt-3.5-turbo-1106
- gpt-3.5-turbo-0125
- gpt-3.5-turbo-1106
- gpt-3.5-turbo-0613
- gpt-3.5-turbo-instruct
- gpt-4
- gpt-4-turbo-preview
- gpt-4-32k
- gpt-4-32k-0314
- gpt-4-32k-0613
- gpt-4-0125-preview
- gpt-4-1106-preview
- gpt-4-vision-preview
- gpt-4-32k
- gpt-4-32k-0314
- gpt-4-32k-0613
- claude-3-opus-20240229
- claude-3-sonnet-20240229
- claude-3-haiku-20240307

请求示例

curl请求示例如下：（$API_KEY替换为WildCard创建的专属API Key）

```
curl https://api.gptsapi.net/v1/chat/completions \-H "Content-Type: application/json" \-H "Authorization: Bearer $API_KEY" \-d '{ "model": "gpt-3.5-turbo-0125", "messages": [ { "role": "user", "content": "Hello!" } ] }'
```

可以使用该接口调用claude-3的模型，接口参数定义和响应结果按照chat/completions封装返回，如下：

```
curl https://api.gptsapi.net/v1/chat/completions \-H "Content-Type: application/json" \-H "Authorization: Bearer $API_KEY" \-d '{ "model": "claude-3-opus-20240229", "messages": [ { "role": "system", "content": "You are a helpful assistant." }, { "role": "user", "content": "Hello!" } ] }'
```

### /v1/messages

Anthropic聊天接口，接口定义参考https://docs.anthropic.com/claude/reference/messages_post

支持模型列表

- claude-3-sonnet-20240229
- claude-3-haiku-20240307

**（注意：该接口暂不支持claude-3-opus-20240229模型，若有需要请使用/v1/chat/completions接口）**

请求示例

curl请求示例如下：（$API_KEY替换为WildCard创建的专属API Key）

```
curl https://api.gptsapi.net/v1/messages \--header "x-api-key: $API_KEY" \--header "anthropic-version: 2023-06-01" \--header "content-type: application/json" \--data \ '{ "model": "claude-3-haiku-20240307", "max_tokens": 1024, "messages": [ {"role": "user", "content": "Hello, world"} ] }'
```

## 嵌入接口（Embeddings）

### /v1/messages

OpenAI嵌入接口，接口定义参考https://platform.openai.com/docs/api-reference/embeddings/create

支持模型列表

- text-embedding-ada-002
- text-embedding-3-small
- text-embedding-3-large

请求示例

curl请求示例如下：（$API_KEY替换为WildCard创建的专属API Key）

```
curl https://api.gptsapi.net/v1/embeddings \-H "Content-Type: application/json" \-H "Authorization: Bearer $API_KEY" \-d '{ "input": "The food was delicious and the waiter...", "model": "text-embedding-ada-002", "encoding_format": "float" }'
```

## 图像接口（Images）

### /v1/images/generations

OpenAI创建图像接口，接口定义参考https://platform.openai.com/docs/api-reference/images/create

支持模型列表

- dall-e-3
- dall-e-2

请求示例

curl请求示例如下：（$API_KEY替换为WildCard创建的专属API Key）

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

curl请求示例如下：（$API_KEY替换为WildCard创建的专属API Key）

```
curl https://api.gptsapi.net/v1/audio/speech \-H "Content-Type: application/json" \-H "Authorization: Bearer $API_KEY" \-d '{ "model": "tts-1", "input": "The quick brown fox jumped over the lazy dog.", "voice": "alloy" }' \ --output speech.mp3
```

