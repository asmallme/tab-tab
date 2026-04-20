# Privacy Policy for Tab Tab

_Last updated: 2026-04-17_

## 简体中文

Tab Tab（以下简称"本扩展"）是一款运行在 Chrome 浏览器内的标签页管理工具。我们非常重视你的隐私。

### 我们收集的信息

**本扩展不收集、不存储、不上传任何用户数据到任何服务器。**

为了实现标签页分组、搜索、最近活跃列表等核心功能，本扩展会在你本地的浏览器中读取以下信息：

- 你当前打开的标签页的标题、URL、favicon
- 你对标签页的切换和关闭行为（用于生成"最近活跃"列表）
- 你的分组偏好设置（置顶、折叠、排序）

所有以上信息仅保存在 Chrome 浏览器本地的 `chrome.storage.local` 中，不会被传输到任何外部服务器，也不会与第三方共享。

### 权限说明

- `tabs`：读取和操作标签页，这是核心功能所必需的
- `storage`：在本地保存你的分组偏好设置
- `favicon`：展示网站图标

### 你的控制权

你可以随时：
- 在 `chrome://extensions/` 禁用或删除本扩展
- 卸载本扩展时，所有本地存储的数据会被自动清除

### 联系方式

如对本隐私政策有任何疑问，请通过 [GitHub Issues](https://github.com/asmallme/tab-tab/issues) 联系我们。

---

## English

Tab Tab is a Chrome extension for managing browser tabs. We take your privacy seriously.

### Information We Collect

**Tab Tab does NOT collect, store, or transmit any user data to any external server.**

To provide its core features (tab grouping, search, recent activity), the extension reads the following locally in your browser:

- The title, URL, and favicon of your currently open tabs
- Your tab switching/closing behavior (to populate the "recently active" list)
- Your group preferences (pinned, collapsed, order)

All of the above is stored only in `chrome.storage.local` on your device and is never transmitted to any server or shared with any third party.

### Permission Justifications

- `tabs`: Required to read and operate on your tabs, which is the core feature.
- `storage`: Required to locally persist your grouping preferences.
- `favicon`: Required to display site icons.

### Your Control

You can at any time:
- Disable or remove the extension at `chrome://extensions/`
- Uninstalling the extension automatically removes all locally stored data.

### Contact

For questions about this policy, please open an issue at [GitHub Issues](https://github.com/asmallme/tab-tab/issues).
