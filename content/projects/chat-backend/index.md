---
title: 聊天后端(441 行 Node 原生)
slug: chat-backend
description: 不用 npm install —— node server.mjs 就能跑的对话后端
date: 2026-09-14
weight: 5
icon: /img/proj_app_server.webp
tags: [Node.js, SSE, 多模态, 开源]
links:
  - title: GitHub
    website: https://github.com/WYR-233/webview-shell
  - title: Gitee
    website: https://gitee.com/wyr233/webview-shell
---

## 极简后端

**441 行 Node 原生代码**,不用 `npm install`,直接 `node server.mjs` 就能跑。没有框架、没有依赖树——十年后打开还能跑。

## 功能

- **SSE 流式对话**:逐字返回,前端体验流畅
- **多模态**:图片直接喂模型
- **内容寻址图床**:上传的图片按内容哈希存,自动去重
- **可选长期记忆**:用 markdown 卡片做跨对话记忆,纯文件、可读可改、方便备份

## 设计取舍

框架能省事,但依赖越少越好维护。这个后端的目标是:**几个文件、几百行代码,自己看得懂、改得动**。

## 入口

[GitHub](https://github.com/WYR-233/webview-shell) / [Gitee](https://gitee.com/wyr233/webview-shell)
