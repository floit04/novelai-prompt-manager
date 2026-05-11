# 提示词助手 悬浮窗 (NovelAI) · Prompt Assistant Float Panel · プロンプト管理 浮動ウィンドウ

> Tampermonkey / Violentmonkey userscript for **NovelAI** — manage, organize, and reuse your prompts in a floating resizable panel.

---

## 目录 / Contents / 目次

- [中文说明](#中文说明)
- [English](#english)
- [日本語](#日本語)

---

## 中文说明

### 简介

**提示词助手 悬浮窗 (NovelAI)** 是一个 Tampermonkey 油猴脚本，在 NovelAI 页面右下角添加一个可拖拽、可缩放的悬浮面板，帮助你管理和复用 AI 绘画提示词。

### 主要功能

| 功能 | 说明 |
|------|------|
| 🗂️ 多工作空间 | 按主题分类管理提示词（通用、角色、衣柜、串串……） |
| 📁 层级分类 | 无限嵌套的分类体系，支持拖拽排序 |
| 🖼️ 三种视图 | 画廊（Gallery）、瀑布流（Masonry）、列表（List）|
| 📷 图片绑定 | 每张提示词卡片可绑定参考图，支持 NAI 元数据自动识别 |
| 📤 发送到 NAI | 一键将图片注入 NovelAI 生成界面 |
| 💾 存档系统 | 最多 10 个 IndexedDB 存档，支持命名/重命名/删除 |
| 🌏 多语言 | 中文 / English / 日本語 切换（设置面板内） |
| 🎨 卡片配色 | 单色/双色渐变背景，色块宽度 100-400px 可调 |
| 📦 ZIP 导入/导出 | 一键备份/还原所有数据 |
<img width="1470" height="1218" alt="image" src="https://github.com/user-attachments/assets/64df38ce-389d-4512-abd1-b7d1eaaee990" />


### 安装

1. 安装 [Tampermonkey](https://www.tampermonkey.net/) 或 [Violentmonkey](https://violentmonkey.github.io/)
2. 将 `提示词助手 悬浮窗 (NovelAI)-1.2.0.user.js` 拖拽到浏览器，点击安装
3. 打开 [novelai.net](https://novelai.net) 即可看到右下角悬浮按钮

### 快捷键

| 快捷键 | 功能 |
|--------|------|
| `Shift + P` | 打开 / 关闭悬浮面板 |

### 数据存储

- **图片 & 状态**：IndexedDB（`PromptImageDB_v6`，版本 4）  
- **存档槽位**：IndexedDB `slots` objectStore（自动从旧版 localStorage 迁移）  
- **视图偏好 / 语言偏好**：`localStorage`

### 更新日志

请见 [CHANGELOG.md](./CHANGELOG.md)

### 许可证

[MIT License](./LICENSE) © 2025

---

## English

### Introduction

**Prompt Assistant Float Panel (NovelAI)** is a Tampermonkey/Violentmonkey userscript that adds a draggable, resizable floating panel to [novelai.net](https://novelai.net), helping you manage, organize, and instantly reuse AI image-generation prompts.

### Features

| Feature | Description |
|---------|-------------|
| 🗂️ Multi-workspace | Organize prompts by theme (General, Characters, Wardrobe, Strings…) |
| 📁 Category hierarchy | Unlimited nested categories with drag-and-drop reordering |
| 🖼️ Three view modes | Gallery, Masonry (waterfall), and List |
| 📷 Image binding | Attach reference images to cards; auto-parses NAI PNG metadata |
| 📤 Send to NAI | One-click image injection into the NAI generation UI |
| 💾 Save slots | Up to 10 named IndexedDB save slots |
| 🌏 Multilingual | zh-CN / English / 日本語 (switcher in settings panel) |
| 🎨 Card colors | Solid or dual-tone gradient backgrounds; card width 100–400 px |
| 📦 ZIP backup | Export/import all data as a ZIP archive |
<img width="1470" height="1218" alt="image" src="https://github.com/user-attachments/assets/f7d50949-7fd3-4c87-bc2d-7103da1d87e1" />


### Installation

1. Install [Tampermonkey](https://www.tampermonkey.net/) or [Violentmonkey](https://violentmonkey.github.io/)
2. Drag `提示词助手 悬浮窗 (NovelAI)-1.2.0.user.js` into your browser and click **Install**
3. Navigate to [novelai.net](https://novelai.net) — the floating button appears at the bottom-right

### Keyboard Shortcut

| Shortcut | Action |
|----------|--------|
| `Shift + P` | Toggle the floating panel |

### Data Storage

- **Images & app state**: IndexedDB (`PromptImageDB_v6`, version 4)  
- **Save slots**: IndexedDB `slots` objectStore (auto-migrated from legacy localStorage)  
- **View / language preferences**: `localStorage`

### Changelog

See [CHANGELOG.md](./CHANGELOG.md)

### License

[MIT License](./LICENSE) © 2025

---

## 日本語

### 概要

**プロンプト管理 浮動ウィンドウ (NovelAI)** は Tampermonkey/Violentmonkey 用のユーザースクリプトです。[novelai.net](https://novelai.net) にドラッグ・リサイズ可能な浮動パネルを追加し、AI 画像生成のプロンプトを管理・再利用できます。

### 主な機能

| 機能 | 説明 |
|------|------|
| 🗂️ マルチワークスペース | テーマ別（汎用・キャラ・衣装・文字列…）に整理 |
| 📁 階層カテゴリ | 無制限ネスト、ドラッグ並び替え対応 |
| 🖼️ 3種ビュー | ギャラリー・ウォーターフォール・リスト |
| 📷 画像バインド | カードに参考画像を添付、NAI PNG メタデータ自動解析 |
| 📤 NAIへ送る | ワンクリックで NAI 生成 UI に画像を注入 |
| 💾 セーブスロット | 最大10件、IndexedDB 保存（命名・削除対応） |
| 🌏 多言語対応 | 中文 / English / 日本語（設定パネルで切替） |
| 🎨 カード配色 | 単色・デュアルトーン背景、幅 100–400 px 調整可 |
| 📦 ZIP バックアップ | 全データを ZIP でエクスポート/インポート |
<img width="1470" height="1218" alt="image" src="https://github.com/user-attachments/assets/2944e461-9c33-4a47-afdc-a816bd03a125" />


### インストール

1. [Tampermonkey](https://www.tampermonkey.net/) または [Violentmonkey](https://violentmonkey.github.io/) をインストール
2. `提示词助手 悬浮窗 (NovelAI)-1.2.0.user.js` をブラウザにドラッグして **インストール** をクリック
3. [novelai.net](https://novelai.net) を開くと右下に浮動ボタンが表示されます

### ショートカットキー

| キー | 動作 |
|------|------|
| `Shift + P` | 浮動パネルの開閉 |

### データ保存先

- **画像・アプリ状態**: IndexedDB（`PromptImageDB_v6`、バージョン 4）  
- **セーブスロット**: IndexedDB `slots` objectStore（旧 localStorage から自動移行）  
- **ビュー・言語設定**: `localStorage`

### 変更履歴

[CHANGELOG.md](./CHANGELOG.md) を参照してください。

### ライセンス

[MIT License](./LICENSE) © 2025
