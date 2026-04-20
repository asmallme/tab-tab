# Privacy Policy for Tab Tab

_Last updated: 2026-04-21_

## 简体中文

Tab Tab（以下简称"本扩展"）是一款运行在 Chrome 浏览器内的标签页管理工具。我们非常重视你的隐私。

### 我们收集的信息

**本扩展不收集、不存储、不上传任何用户数据到任何服务器。**

为了实现标签页分组、搜索、最近活跃、最近关闭、会话保存等核心功能，本扩展会在你本地的浏览器中读取以下信息：

- 你当前打开的标签页的标题、URL、favicon、静音/发声状态、所属窗口与原生分组
- 你对标签页的切换、关闭行为（用于生成"最近活跃"与"最近关闭"列表）
- 你的分组偏好设置（分组模式、置顶、折叠、排序）、自定义分组、保存的会话
- 你在"设置"中自定义的阈值（休眠时长、僵尸天数等）

所有以上信息**仅保存在 Chrome 浏览器本地的 `chrome.storage.local`** 中，不会被传输到任何外部服务器，也不会与第三方共享。卸载本扩展时，这些数据会被 Chrome 自动清除。

本扩展**不使用任何远程代码**，不加载外部脚本，不接入任何分析 / 埋点 / 广告 SDK。

### 权限说明

| 权限 | 用途 |
|---|---|
| `tabs` | 读取标签页的标题 / URL / favicon，以及激活、关闭、静音、休眠、移动标签页。这是实现分组、搜索、批量操作的基础能力。 |
| `tabGroups` | 读取与写入 Chrome 原生 Tab Groups。用于"按原生分组"视图，以及将自定义分组一键同步为原生分组（含颜色、名称）。 |
| `sessions` | 读取 `chrome.sessions.getRecentlyClosed`，展示"最近关闭"列表；调用 `chrome.sessions.restore` 恢复关闭的标签页。 |
| `storage` | 在本地保存你的分组偏好、自定义分组、会话、最近关闭快照、设置项。 |
| `favicon` | 通过 Chrome 内置 favicon 服务展示网站图标（当 `favIconUrl` 为空时作为兜底）。 |
| `downloads` | 在"设置"中"导出 JSON 配置"时，把配置文件保存到你指定的位置。仅在你主动点击导出时触发，不会自动下载任何文件。 |

本扩展**不申请 `host_permissions`**，不会读取任何网页的具体内容（DOM、Cookie、表单等）。

### 你的控制权

你可以随时：
- 在 `chrome://extensions/` 禁用或删除本扩展
- 在扩展内"设置 → 导出 JSON 配置"备份本地数据
- 卸载本扩展，所有本地存储的数据会被自动清除

### 数据的用途（合规声明）

我们声明，本扩展收集到的上述信息：

- **不**用于与扩展单一目的无关的任何用途
- **不**出售给第三方
- **不**用于或转让给任何广告、信用评分或放贷用途
- **不**用于身份识别、跟踪用户跨站点行为

### 变更

如本政策有更新，我们会修改本文件顶部的 "Last updated" 日期，并在新版本扩展的更新说明中注明。

### 联系方式

如对本隐私政策有任何疑问，请通过 [GitHub Issues](https://github.com/asmallme/tab-tab/issues) 联系我们。

---

## English

Tab Tab is a Chrome extension for managing browser tabs. We take your privacy seriously.

### Information We Collect

**Tab Tab does NOT collect, store, or transmit any user data to any external server.**

To provide its core features (tab grouping, search, recently active, recently closed, session saving), the extension reads the following **locally** in your browser:

- Title, URL, favicon, audible/muted state, owning window and native group of your currently open tabs
- Your tab switching and closing behavior (to populate the "recently active" and "recently closed" lists)
- Your group preferences (group mode, pinned, collapsed, order), custom groups and saved sessions
- Thresholds you configured in Settings (e.g. hibernate hours, zombie days)

All of the above is stored **only in `chrome.storage.local` on your device**, is never transmitted to any server, and is never shared with any third party. Uninstalling the extension clears this data automatically.

The extension uses **no remote code**, loads no external scripts, and includes **no analytics / telemetry / advertising SDKs**.

### Permission Justifications

| Permission | Purpose |
|---|---|
| `tabs` | Read tab title / URL / favicon and perform activate, close, mute, discard (hibernate), move operations. Core capability for grouping, searching, and bulk actions. |
| `tabGroups` | Read & write Chrome native Tab Groups. Powers the "Native groups" view and the one-click "sync custom groups to native groups" feature (with color and name). |
| `sessions` | Read `chrome.sessions.getRecentlyClosed` to render the "Recently closed" list, and call `chrome.sessions.restore` to restore closed tabs. |
| `storage` | Locally persist group preferences, custom groups, saved sessions, recently-closed snapshots, and settings. |
| `favicon` | Show site favicons via Chrome's built-in favicon service (fallback when `favIconUrl` is empty). |
| `downloads` | When you click "Export JSON config" in Settings, save the config file to the location you choose. Only triggered by explicit user action; nothing is downloaded automatically. |

The extension requests **no `host_permissions`** and does not read the content (DOM, cookies, form fields, etc.) of any web page.

### Your Control

At any time you can:
- Disable or remove the extension at `chrome://extensions/`
- Export your local data via Settings → "Export JSON config"
- Uninstall the extension, which clears all locally stored data automatically

### Data Use Disclosures

We certify that:

- We **do not** use the collected information for any purpose unrelated to the extension's single purpose
- We **do not** sell data to third parties
- We **do not** use or transfer the data for advertising, creditworthiness, or lending purposes
- We **do not** use the data to identify users or track them across sites

### Changes

If this policy is updated, we will change the "Last updated" date at the top of this document and mention the change in the release notes of the next version.

### Contact

For questions about this policy, please open an issue at [GitHub Issues](https://github.com/asmallme/tab-tab/issues).
