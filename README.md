# 🎧 ListenFlow (听流)

**专为 Microsoft Edge "大声朗读" 打造的沉浸式听书 Web App。**

> 解决痛点：普通阅读器在 Edge 中读完一章会自动停止。ListenFlow 通过智能拼接技术，实现“一次点击，畅听 2 小时”的连贯体验。

## ✨ 核心特性

* **🚗 司机/通勤友好**：独创的“批量加载模式” (Batch Loading)，一次渲染 20 个章节，避免频繁手动翻页，实现真正的免提听书。
* **🗣️ Edge TTS 深度优化**：重构 DOM 结构，去除页眉页脚和广告干扰，只保留纯净文本，让 Edge 的神经语音（如 Cloud Yunxi）朗读更丝滑。
* **🧹 智能清洗**：自动检测并移除重复的章节标题和乱码，提供像电台文案一样的阅读流。
* **🔒 隐私安全**：基于 `epub.js` 开发，所有解析均在浏览器本地完成（Client-side only），书籍文件不会上传到任何服务器。
* **⚡️ 极速体验**：使用 CDN 加速核心库，支持 PWA 级别的离线访问体验。

## 🚀 如何使用

1. 使用 **Microsoft Edge** 浏览器打开网页。
2. 点击上传 `.epub` 电子书。
3. 点击底部 **"下一组"** 加载章节。
4. 点击 Edge 地址栏的 **"大声朗读" (A)** 图标，锁屏即可开始听书。

## 🛠 技术栈

* HTML5 / CSS3
* Vanilla JavaScript (无框架依赖)
* [epub.js](https://github.com/futurepress/epub.js) - 核心解析库
* [JSZip](https://github.com/Stuk/jszip) - 解压支持
