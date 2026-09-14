---
title: 手机端页面(一个 HTML 就是界面)
slug: mobile-web
description: 不用 npm、不用打包器 —— 单个 HTML 文件承载完整聊天界面
date: 2026-09-14
weight: 4
icon: /img/proj_app_web.webp
tags: [前端, 流式输出, 开源]
links:
  - title: GitHub
    website: https://github.com/WYR-233/webview-shell
  - title: Gitee
    website: https://gitee.com/wyr233/webview-shell
---

## 一个文件就是全部界面

没有 npm、没有打包器、没有构建步骤——**一个 HTML 文件**,丢到任意静态服务器就能用。

## 功能

- **流式回复**:边生成边显示,不用等整段
- **发图自动压缩上传**:手机拍照直接发,不卡流量
- **亮暗双主题**:跟随系统设置
- **图片查看器**:点开大图、手势缩放

## 为什么这样做

移动端调试成本高,前端越简单越好维护。没有构建链意味着:**改一行、刷新页面**就生效,出问题也好定位。

## 入口

[GitHub](https://github.com/WYR-233/webview-shell) / [Gitee](https://gitee.com/wyr233/webview-shell)
