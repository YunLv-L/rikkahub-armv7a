<div align="center">
  <img src="docs/icon.png" alt="App Icon" width="100" />
  <h1>RikkaHub</h1>

[![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/rikkahub/rikkahub)
[![Ask DeepWiki](https://img.shields.io/badge/zread.ai-blue?style=flat&logo=readthedocs)](https://zread.ai/rikkahub/rikkahub)

A native Android LLM chat client that supports switching between different providers for
conversations 🤖💬

**📌 ARMv7a 适配版 | ARMv7a Adapted Version**

> 本仓库为 ARMv7a（32 位）设备提供持续更新的 RikkaHub 版本，基于官方最新源码构建，功能与官方版本完全一致。官方从 0.0.9 开始已不再提供 ARMv7a 支持。
>
> This repository provides continuously updated RikkaHub builds for ARMv7a (32-bit) devices, based on the latest official source code with identical functionality. Official support for ARMv7a was dropped starting from version 0.0.9.

Click to join our Discord server 👉 [【RikkaHub】](https://discord.gg/9weBqxe5c4)

[简体中文](README_ZH_CN.md) | [繁體中文](README_ZH_TW.md) | English | [ARMv7a 适配说明](README_ARMV7A.md)
</div>

<div align="center">
  <img src="docs/img/chat.png" alt="Chat Interface" width="150" />
  <img src="docs/img/desktop.png" alt="Models Picker" width="450" />
</div>

## 🚀 Download

### 📱 ARMv7a 版本下载 | ARMv7a Build Download

**GitHub Releases（本仓库）：**
👉 [https://github.com/YunLv-L/rikkahub-armv7a/releases](https://github.com/YunLv-L/rikkahub-armv7a/releases)

> 此版本适用于 ARMv7a（32 位）设备，如旧款 Android 手机。安装前请先卸载官方版本（签名不同，无法直接覆盖）。
>
> This version is for ARMv7a (32-bit) devices. Please uninstall the official version before installing (signatures differ).

### 🔗 官方版本 | Official Builds

🔗 [Download from Website](https://rikka-ai.com/download) (Recommended)

🔗 [Download from Google Play](https://play.google.com/store/apps/details?id=me.rerere.rikkahub)

## 💖 Sponsors

|                                         Sponsor                                         | Description                                                                                                                                                                                                                                         |
|:---------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <img src="docs/sponsors/aihubmix.png" alt="Aihubmix" width="50" /><br /><b>Aihubmix</b> | Thanks to <a href="https://aihubmix.com?aff=pG7r">aihubmix.com</a> for their financial support. We recommend using aihubmix as a one-stop shop for mainstream models worldwide. (OpenAI, Claude, Google Gemini, DeepSeek, Qwen, and hundreds more). |
| <img src="docs/sponsors/suixiang.jpg" alt="随想AI网关" width="50" /><br /><b>随想AI网关</b> | 感谢随想AI网关对本项目的赞助！随想AI网关 是一家可靠高效的 API 中继服务提供商，提供 Claude、Codex、Gemini 等的中继服务。注重隐私的中转站·无数据倒卖·无模型掺水，隐私，透明，极速售后。新账户注册每日签到就送 0.5 元测试额度，充值额度 1:1，无需订阅，按量付费。多线路冗余、跨区域容灾、自动故障切换，长链路 SSE 不中断。99.9% 可用性，关键调用从不掉队。 |

> 以上赞助为官方 RikkaHub 项目所有，本 ARMv7a 适配版不涉及任何商业赞助。  
> The above sponsors belong to the official RikkaHub project; this ARMv7a adaptation does not involve any commercial sponsorship.

## ✨ Features

- 🎨 Material You Design and 🌙 Dark mode
- 📦 Workspace: a proot-based Linux agent environment
- 🔄 Multiple AI Provider Support: custom API / URL / models (all OpenAI, Google, Anthropic compatible api)
- 🖼️ Multimodal input support (Image, Text Documentation, PDF, Docx)
- 🖥️ Web access for multi-platform use
- 🛠️ MCP support
- 📝 Markdown Rendering (with code highlighting, Latex formulas, tables, Mermaid)
- 🪾 Message Branching
- 🔍 Search capabilities (Exa, Tavily, Zhipu, LinkUp, Brave, Perplexity, etc.)
- 🧩 Prompt variables (model name, time, etc.)
- 🤳 QR code export and import for providers
- 🤖 Agent customization
- 🧠 ChatGPT-like memory feature
- 📝 AI Translation
- 🌐 Custom HTTP request headers and request bodies
- 💌 Silly Tavern character card import

## ⚠️ 注意事项 | Notes

### MCP 服务器别名命名限制 | MCP Server Alias Naming Restriction

从 v2.3.0 版本开始，RikkaHub 对 MCP 服务器别名（Alias）增加了格式校验。别名**只能包含英文字母、数字、下划线 `_` 和连字符 `-`**，不允许包含空格或其他特殊字符。

如果别名包含非法字符（如空格、中文、标点等），连接 MCP 服务器时会报以下错误：

```
retrofit2.HttpException: Invalid 'tools[2].function.name': string does not match pattern. 
Expected a string that matches the pattern '^[a-zA-Z0-9_-]+$'.
```

**解决方法：** 将别名修改为合法格式，例如 `MT Manager` 改为 `MT-Manager` 或 `MT_Manager`。

---

> **Note:** Since v2.3.0, RikkaHub validates MCP server alias names. Aliases may only contain **letters, numbers, underscores `_`, and hyphens `-`**. Spaces and other special characters are not allowed.
>
> If your alias contains invalid characters, you will see the error above. Rename it to a valid format (e.g., change `MT Manager` to `MT-Manager` or `MT_Manager`).

## ✨ Contributing

This project is developed using [Android Studio](https://developer.android.com/studio). PRs are
welcome!

Technology stack documentation:

- [Kotlin](https://kotlinlang.org/) (Development language)
- [Koin](https://insert-koin.io/) (Dependency Injection)
- [Jetpack Compose](https://developer.android.com/jetpack/compose) (UI framework)
- [DataStore](https://developer.android.com/topic/libraries/architecture/datastore) (Preference data
  storage)
- [Room](https://developer.android.com/training/data-storage/room) (Database)
- [Coil](https://coil-kt.github.io/coil/) (Image loading)
- [Material You](https://m3.material.io/) (UI design)
- [Navigation 3](https://developer.android.com/guide/navigation/navigation-3) (Navigation)
- [Okhttp](https://square.github.io/okhttp/) (HTTP client)
- [kotlinx.serialization](https://github.com/Kotlin/kotlinx.serialization) (JSON serialization)

> [!TIP]
> You need a `google-services.json` file at `app` folder to build the app.

> [!IMPORTANT]  
> The following PRs will be rejected:
> 1. Translation related changes, such as adding new languages or updating existing translations
> 2. Adding new features, this project is opinionated and will not accept pull requests for new features
> 3. Large-scale refactoring and changes generated by AI

## 💰 Donate

本 ARMv7a 适配版不接受捐赠，如果你希望支持 RikkaHub 的开发，请直接向官方项目捐赠：

This ARMv7a adaptation does not accept donations. If you wish to support RikkaHub development, please donate to the official project:

* [Patreon](https://patreon.com/rikkahub)
* [爱发电](https://afdian.com/a/reovo)

## ⭐ Star History

If you like this project, please give it a star ⭐

![Star History Chart](https://api.star-history.com/svg?repos=re-ovo/rikkahub,YunLv-L/rikkahub-armv7a&type=Date)

> 上图同时展示官方仓库（re-ovo/rikkahub）与本 ARMv7a 适配仓库（YunLv-L/rikkahub-armv7a）的 Star 增长趋势。  
> The chart above shows the Star history of both the official repository (re-ovo/rikkahub) and this ARMv7a adapted repository (YunLv-L/rikkahub-armv7a).

## 📄 License

[License](LICENSE)
