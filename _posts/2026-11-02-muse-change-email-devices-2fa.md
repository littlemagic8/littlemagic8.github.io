---
layout:     post
title:      Muse 如何更换登录邮箱、删除旧设备并开启 2FA？完整教程
subtitle:   在 Muse 的 Meta Account 中添加新邮箱、退出陌生设备，并用验证器保护登录
date:       2026-11-02
author:     aicygg888
header-img: img/post-bg-cook.jpg
catalog: true
tags:
    - Muse
    - Meta Account
    - 账户安全
    - 2FA
---

Muse 的登录、联系邮箱和安全设置由 **Meta Account** 管理。更换邮箱、清理不再使用的设备、开启两步验证，都可以从 Muse 的设置中进入同一个账户中心完成。

本文以网页版界面为例。不同地区和版本的菜单名称可能略有变化；操作前请确认登录的是需要管理的 Muse 账号，并确保新邮箱和验证器都由自己控制。

> **重要：**更换邮箱时，先添加并验证新邮箱，再删除旧邮箱；开启 2FA 后请妥善保存恢复代码。不要把密码、恢复代码或验证器密钥提交到陌生网页。

## 一、查看 Muse 账号额度并进入 Meta Account

### 查看账号拥有的额度

在 Muse 左下角打开 **Settings（设置）**，停留在 **General（通用）** 页面。在 **Usage（用量）** 区域可以查看免费套餐的重置时间，以及账号已拥有的额外 Token 余额；图中箭头标注的位置显示为 **1B tokens left**。

![查看 Muse 账号拥有的 Token 额度](/img/2026-11-02-muse-account-security/10亿token查看.png)

### 进入 Meta Account

同一页面顶部的 **Meta Account** 入口用于管理登录邮箱、设备和账户安全。点击后会在新窗口打开账户设置。

如果界面是英文，可以先在 **Language（语言）** 中切换为简体中文，后面的菜单更容易对应。

![Muse 设置语言为简体中文](/img/2026-11-02-muse-account-security/设置简体中文.png)

进入后，在左侧选择 **Login and security（登录和安全）**。邮箱、已登录设备和两步验证都从这里管理。

![Meta Account 的登录和安全页面](/img/2026-11-02-muse-account-security/登录和安全.png)

## 二、如何更换 Muse 登录邮箱

Meta Account 支持先添加新的联系方式，再移除旧邮箱。这样可以避免删除后收不到确认邮件，或因旧邮箱失效而无法登录。

### 第一步：打开联系方式

在 **Login and security（登录和安全）** 中，找到账号资料里的联系方式设置，点击进入当前邮箱。

![打开账户联系方式](/img/2026-11-02-muse-account-security/点击设置账户信息.png)

进入 **Contact info（联系方式）** 后，点击 **Add new contact info（添加新的联系方式）**。

![添加新的联系方式](/img/2026-11-02-muse-account-security/添加新的账号信息.png)

### 第二步：添加并验证新邮箱

选择添加邮箱，填写准备长期使用、能够正常收信的新邮箱地址。

![添加新的邮箱](/img/2026-11-02-muse-account-security/添加新的邮箱.png)

Meta 会向新邮箱发送验证码。打开新邮箱，填写收到的验证码完成验证。

![填写新邮箱验证码](/img/2026-11-02-muse-account-security/填写新邮箱验证码.png)

页面显示新邮箱已添加后，先不要急着删除旧邮箱。建议退出后用新邮箱完成一次登录确认。

![确认新邮箱添加成功](/img/2026-11-02-muse-account-security/新邮箱添加成功.png)

### 第三步：确认新邮箱可用后，移除旧邮箱

返回邮箱列表，选择准备移除的旧邮箱。

![选择要移除的旧邮箱](/img/2026-11-02-muse-account-security/选择要移除的邮箱账号.png)

点击 **Delete email（删除邮箱）**。

![点击删除邮箱](/img/2026-11-02-muse-account-security/点击删除邮箱.png)

阅读弹窗提示后确认删除。若此邮箱仍是唯一可用的登录或恢复方式，系统可能不允许直接移除；此时请先确认新邮箱已经验证成功。

![确认删除旧邮箱](/img/2026-11-02-muse-account-security/确认删除.png)

删除后，检查列表中是否只保留需要使用的邮箱。

![确认只保留一个登录邮箱](/img/2026-11-02-muse-account-security/查看只剩下一个账号.png)

## 三、如何删除之前登录过的设备

如果账号曾在旧电脑、共享设备或不认识的浏览器登录过，建议立刻检查会话并退出。退出设备后，该设备下次继续使用 Muse 时需要重新登录。

### 第一步：查看登录设备

在 **Login and security（登录和安全）** 页面，打开 **Where you're logged in（登录位置）**，查看已登录的设备和浏览器。

![查看当前登录设备](/img/2026-11-02-muse-account-security/查看在哪些设备登录.png)

### 第二步：退出单台旧设备

选择不再使用或无法确认的设备，点击退出登录。

![选择需要退出的设备](/img/2026-11-02-muse-account-security/选择设备登出.png)

在确认框中选择 **Log out（退出）**。

![确认退出指定设备](/img/2026-11-02-muse-account-security/确认登出.png)

### 第三步：需要时退出所有设备

如果无法判断哪些会话可信，选择 **Log out of all devices（退出所有设备）** 更稳妥。执行后，你自己的电脑和手机也会被退出，需要使用新邮箱、密码和 2FA 再次登录。

![选择退出所有设备](/img/2026-11-02-muse-account-security/选择登出所有设备.png)

完成后回到设备列表，确认只留下自己正在使用的设备。

![确认只剩当前设备登录](/img/2026-11-02-muse-account-security/确认只有一台设备登录.png)

## 四、如何开启 2FA 两步验证

两步验证会在新设备或新浏览器登录时，要求额外输入一次性验证码。Meta 也建议为陌生设备登录增加这一层保护。[查看 Meta 官方账户安全说明](https://www.meta.com/zh-cn/safety/topics/safety-basics/tools/security/)

### 第一步：进入安全检查

在 Meta Account 首页或 **Login and security（登录和安全）** 中打开 **Meta Security Checkup（安全检查）**。

![打开 Meta Security Checkup](/img/2026-11-02-muse-account-security/安全检查.png)

选择两步验证，并按页面提示设置验证方式。优先选择自己手机中的可信验证器 App；设置完成后，请保存系统提供的恢复代码，并保存在密码管理器或其他安全位置。

### 第二步：完成当前身份验证

开启或修改安全设置时，系统会要求再次确认身份。选择已经绑定的验证器 App，或在确实无法使用验证器时选择恢复代码，然后点击 **Next（下一步）**。

![选择验证器或恢复代码确认身份](/img/2026-11-02-muse-account-security/验证2fa.png)

下图只是一次性验证码的操作示意。**请不要把 2FA 密钥、恢复代码或完整账号信息输入第三方在线工具；应直接在自己的验证器 App 中查看动态验证码。**

![一次性验证码示意](/img/2026-11-02-muse-account-security/通过2fa.fun接收验证码.png)

### 第三步：用新设备登录时输入验证码

以后在新设备打开 Muse 时，先填写账号登录信息。

![填写 Muse 账号登录信息](/img/2026-11-02-muse-account-security/填写账号登录.png)

如需邮箱验证，按提示输入邮箱验证码。

![填写邮箱验证码](/img/2026-11-02-muse-account-security/填写邮箱验证码.png)

开启 2FA 后，再从自己的验证器 App 获取当前动态验证码并填写，完成登录。

![填写 2FA 验证码完成登录](/img/2026-11-02-muse-account-security/填写接收的2fa验证码进行登录.png)

## 五、操作完成后检查这 4 项

- 新邮箱已经验证，可以正常收到登录或安全通知。
- 旧邮箱已经移除，或至少不再是唯一恢复方式。
- 设备列表中没有陌生设备；需要时已退出所有设备。
- 2FA 已开启，恢复代码已单独保存，并且没有泄露验证器密钥。

## 想体验更多 AI 产品？

Muse 的账号安全设置完成后，如果你也需要 ChatGPT Plus、Claude Pro 等 AI 服务，可以访问我们的 [AI 服务自助平台](https://littlemagic8.github.io/gptplus/)，页面提供可购买的充值商品和使用说明。

想直接为自己的 ChatGPT 账号开通 Plus，也可查看 [ChatGPT Plus 自助充值商品](https://littlemagic8.github.io/gptplus/purchase-gpt.html)。遇到使用问题，可添加微信 **aicygg888**，备注：**GPT代充**。
