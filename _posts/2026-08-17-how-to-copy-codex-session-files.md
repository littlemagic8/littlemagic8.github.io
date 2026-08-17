---
layout:     post
title:      怎么拷贝迁移 ChatGPT(Codex) 本地会话数据，三种平台（Windows / macOS / Linux）之间任意拷贝迁移
subtitle:   只搬 sessions，不要动 auth.json
date:       2026-08-17
author:     aicygg888
header-img: img/post-bg-cook.jpg
catalog: true
tags:
    - Codex
    - Codex CLI
    - ChatGPT Plus
---

换电脑、家里和公司两台机器来回写代码，最烦的是 Codex CLI 里那串对话没了：方案、踩过的坑、改到一半的仓库上下文，全得重讲一遍，本文教你如何迁移codex对话数据，

> ps: 只拷codex会话文件即可。登录文件 `auth.json` 不要动。

> Codex 订阅 ChatPlus / Pro就又会更多额度，如需国内支付宝 / 微信自助代充开通ChatPlus / Pro可以参考本教程：
>
> **[一分钟搞定 ChatGPT Plus 充值，ChatGPT Plus【代充值】自助订阅手把手教程](https://littlemagic8.github.io/2026/08/16/how-to-sub-gptplus/)** ：[https://littlemagic8.github.io/2026/08/16/how-to-sub-gptplus/](https://littlemagic8.github.io/2026/08/16/how-to-sub-gptplus/)

| 系统 | 会话目录 |
| :--- | :--- |
| Windows 原生 | `%USERPROFILE%\.codex\sessions` |
| macOS / Linux / WSL | `~/.codex/sessions` |

目录必须保持 `YYYY\MM\DD\rollout-*.jsonl`，不要打乱。

## 拷之前先确认源文件数量

**作用：** 在旧电脑上数有多少条会话文件。后面拷完要用这个数字对照。`Count` 是 `0` 就停，先分清自己用的是原生 Windows 还是 WSL，目录不是同一套。

Windows PowerShell：

```powershell
Get-ChildItem "$env:USERPROFILE\.codex\sessions" -Recurse -Filter "rollout-*.jsonl" | Measure-Object | Select-Object Count
```

- `Get-ChildItem`：列出 `sessions` 里所有文件，`-Recurse` 连子目录一起找，`-Filter` 只看 `rollout-*.jsonl`（真正的对话文件）。
- `Measure-Object`：统计找到了多少个。
- `Select-Object Count`：只打印数量。

![确认 Windows 会话文件数量](/img/2026-08-17-how-to-copy-codex-session-files/image-20260817224114867.png)

macOS / Linux / WSL：

```bash
find ~/.codex/sessions -name 'rollout-*.jsonl' | wc -l
```

- `find ... -name`：在 `~/.codex/sessions` 下找出所有会话文件。
- `wc -l`：数有多少行，也就是多少个文件。

接下来，展示三种情况下codex对话数据如何拷贝复制

## Windows → Windows

### 第一步：拷贝 Codex sessions 对话数据

在**旧电脑**上，把整个 `sessions` 目录拷到 U 盘（或网盘同步盘）。`E:` 按你的 U 盘盘符改。

PowerShell：

```powershell
Copy-Item -Recurse -Force "$env:USERPROFILE\.codex\sessions" "E:\backup\codex-sessions"
```

- `Copy-Item`：复制文件或文件夹。
- `-Recurse`：连年 / 月 / 日三级目录一起拷，不要只拷最外层空壳。
- `-Force`：目标已有同名目录时覆盖。

不用命令、只用资源管理器：

1. 旧电脑按 `Win + R`，粘贴 `%USERPROFILE%\.codex`，回车。
2. 看到 `sessions` 文件夹。整个文件夹复制（不要只进里面挑几个 `jsonl`）。
3. 粘贴到 U 盘或网盘，例如 `E:\backup\codex-sessions`。拷完后 U 盘里应能看到 `2026\08\17\rollout-....jsonl` 这种年 / 月 / 日结构。

### 第二步：还原到新电脑

新电脑上先建好 `.codex`，再把备份还原回去。

PowerShell：

```powershell
New-Item -ItemType Directory -Force -Path "$env:USERPROFILE\.codex" | Out-Null
Copy-Item -Recurse -Force "E:\backup\codex-sessions" "$env:USERPROFILE\.codex\sessions"
```

- `New-Item`：如果新电脑还没有 `.codex` 文件夹，就建一个。
- `| Out-Null`：不刷屏，只做事。
- 第二条 `Copy-Item`：把 U 盘里的备份还原成 `%USERPROFILE%\.codex\sessions`。

资源管理器：

1. 新电脑 `Win + R` → `%USERPROFILE%\.codex`。没有这个文件夹就先新建 `.codex`。
2. 把 U 盘里的 `sessions` 整个贴进去，最终路径必须是：

```text
C:\Users\你的用户名\.codex\sessions\YYYY\MM\DD\rollout-*.jsonl
```

两台都是 Windows，但旧电脑用 WSL、新电脑也用 WSL：不要走上面的 `C:\Users\...`，在 **WSL 终端**里按 macOS / Linux 那一节拷 `~/.codex/sessions`。

## macOS / Linux → macOS / Linux

### 第一步：拷贝 Codex sessions 对话数据

在**旧电脑**上确认会话目录在，再拷走。`user@new-host` 换成新机器的用户名和地址。

先看目录在不在：

```bash
ls ~/.codex/sessions
```

- `ls`：列出 `sessions` 下的年 / 月 / 日目录。这里是空的就先别拷。

**有 SSH 时，在旧电脑直接传到新电脑：**

```bash
ssh user@new-host "mkdir -p ~/.codex"
scp -r ~/.codex/sessions user@new-host:~/.codex/
```

- `ssh ... "mkdir -p ~/.codex"`：登录新机器，没有 `.codex` 就建；`-p` 表示目录已存在也不报错。
- `scp -r`：远程拷贝整个目录。拷完后新机器上是 `~/.codex/sessions`。

同一局域网、机器一直开着，也可以用 `rsync`，中断了能续传：

```bash
rsync -av ~/.codex/sessions/ user@new-host:~/.codex/sessions/
```

- `rsync`：同步目录，适合文件多、中途断过的情况。
- `-a`：保留目录结构和时间。
- `-v`：打印进度。
- 源路径末尾的 `/`：同步 `sessions` **里面的内容**到对面的 `sessions/`，不会多套一层文件夹。

**没有 SSH 时，在旧电脑打成压缩包，再拷到 U 盘或网盘：**

```bash
cd ~
zip -r sessions.zip .codex/sessions
```

- `zip -r`：把整个 `sessions` 目录打进 `sessions.zip`，年 / 月 / 日结构会一起进去。

### 第二步：还原到新电脑

用 `scp` / `rsync` 传过的，新电脑上已经是 `~/.codex/sessions`，执行下面这条确认结构一致：

```bash
ls ~/.codex/sessions
```

用 zip 传的，在新电脑解压到家目录（不要解成 `~/.codex/sessions/sessions`）：

```bash
mkdir -p ~/.codex
unzip sessions.zip -d ~
```

- `mkdir -p ~/.codex`：没有 `.codex` 就建。
- `unzip ... -d ~`：zip 里是 `.codex/sessions/...` 时，解压到家目录后路径正好是 `~/.codex/sessions`。

最终路径必须是：

```text
~/.codex/sessions/YYYY/MM/DD/rollout-*.jsonl
```

## Windows ↔ macOS / Linux

没有一条通用命令能直接跨系统拷。使用远程Xshell、MobaXterm等工具进行文件传输，再解到目标机对应目录。

Windows 解到：

```text
C:\Users\你的用户名\.codex\sessions
```

macOS / Linux / WSL 解到：

```text
~/.codex/sessions
```

WSL 和 Windows 原生是两套目录，不要互拷。

## 拷完怎么验

**作用：** 在新机器再数一遍文件。数量必须和旧电脑刚才记下的 `Count` / `wc -l` 一致。

Windows：

```powershell
Get-ChildItem "$env:USERPROFILE\.codex\sessions" -Recurse -Filter "rollout-*.jsonl" | Measure-Object | Select-Object Count
```

macOS / Linux / WSL：

```bash
find ~/.codex/sessions -name 'rollout-*.jsonl' | wc -l
```

数量对了，再抽一条文件路径出来，用记事本或 `type` / `cat` 打开，确认里面是文本，不是 0 字节空文件。

Windows（只打印第一条路径，不打开内容）：

```powershell
Get-ChildItem "$env:USERPROFILE\.codex\sessions" -Recurse -Filter "rollout-*.jsonl" | Select-Object -First 1 -ExpandProperty FullName
```

- `-First 1`：只要找到的第一条。
- `-ExpandProperty FullName`：打印完整路径，方便你去打开核对。

macOS / Linux / WSL：

```bash
find ~/.codex/sessions -name 'rollout-*.jsonl' | head -1
```

- `head -1`：只输出找到的第一条路径。

打开后应能看到 JSON 文本。路径在、文件是空的，说明拷坏了，重新拷。

## 拷完之后，怎么在 Codex 里看历史对话

文件拷对了，还要用官方命令打开选择器。新电脑先自己登录（不要拷 `auth.json`）：

```bash
codex login
```

**作用：** 在新机器上登录你的 ChatGPT 账号。会话文件和登录态是分开的。

然后看历史：

```bash
codex resume --all
```

**作用：** 打开官方会话选择器，并跨目录搜索全部本地会话。搬家后项目路径经常变了，只用 `codex resume` 或 `codex resume --last` 可能看不到迁过来的记录。

在列表里用方向键选一条，回车即可继续那条对话。

已经进了 Codex 界面时，在输入框敲：

```text
/resume
```

**作用：** 和 `codex resume` 一样，弹出已保存会话列表，不用退出当前窗口。

同一仓库、确认还在原来的项目目录里，才用：

```bash
codex resume --last
```

**作用：** 直接打开「当前目录」最近一次会话，不弹完整列表。目录对不上会误以为对话丢了，优先用 `--all`。

列表是空的，先确认 `codex` 命令能跑，再跑诊断：

```bash
codex --version (如果无法显示，直接拷贝错误信息让AI解决！！)
codex doctor
```

- `codex --version`：确认 CLI 已装进 PATH，至少 **0.30.0** 才有 `resume`。
- `codex doctor`：检查安装、登录、会话清单。还是空的，再核对 `sessions` 是不是拷到了另一套目录（Windows 原生 vs WSL）

## Codex 要用 Plus / Pro，国内怎么订？

会话拷过去了，额度还是挂在 ChatGPT 账号上。没 Plus / Pro，或者额度老触顶，先把订阅搞定。

国内支付宝 / 微信自助开通（卡密 + 登录会话，不用自己绑国际卡）：

**[https://littlemagic8.github.io/2026/08/16/how-to-sub-gptplus/](https://littlemagic8.github.io/2026/08/16/how-to-sub-gptplus/)**

入口也可以直接打开：[https://littlemagic8.github.io/gptplus/purchase-gpt.html](https://littlemagic8.github.io/gptplus/purchase-gpt.html)

Pro / Codex 加量不清楚选哪档，微信 **aicygg888** / **aicygg789** 说一下用途即可。

---

## 联系我们

拷文件卡住、登录不上或要充值，直接找我们。

请保存网址 [https://littlemagic8.github.io/gptplus/](https://littlemagic8.github.io/gptplus/) ，并加上联系方式，防止失联。

防失联客服微信：

```
aicygg888
```

添加好友请备注：**GPT代充**（加的人多，微信防频繁，请扫码）

欢迎加微信：

![微信客服](/img/2026-08-02-x-premium-plus/wechat-qr.png)

公众号也可以哦：

![公众号](/img/v2-4e622b64238b20948a02e0c988ca5704_720w.png)
