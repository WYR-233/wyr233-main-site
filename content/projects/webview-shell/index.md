---
title: 网页变 App 三件套
slug: webview-shell
description: 把自建网页服务变成手机上的真 App —— WebView 壳 + 手机端页面 + Node 后端,三部分一个仓库
date: 2026-09-14
image: /img/cover_proj_webview.webp
weight: 3
icon: /img/proj_app_phone.webp
tags: [Android, WebView, Node.js, 推送, 开源]
links:
  - title: GitHub
    website: https://github.com/WYR-233/webview-shell
  - title: Gitee
    website: https://gitee.com/wyr233/webview-shell
---

## 这是什么

一套「把自己搭的网页服务变成手机 App」的完整方案:**独立图标、全屏无地址栏、能调相册相机、关屏也能收到消息推送**。整套东西零第三方依赖,全部可自托管。

一个仓库三部分:Android 壳、手机端页面、聊天后端——可以整套用,也可以只拿其中一块。

## ① Android 壳:把网页装进真正的 App

- **自己做推送,不依赖厂商通道**:手写 RFC6455 WebSocket 长连接 + 前台服务保活;国产 ROM(小米 / 华为 / vivo / 联想)的保活引导都写在文档里
- **Android 15 适配**:前台服务类型、键盘避让、返回键与页面抽屉的冲突处理
- **WebView 的真实坑**:某些 WebView 不保存 cookie、页面缓存不刷新——都有对应处理

## ② 手机端页面:一个 HTML 就是界面

- 不用 npm、不用打包器,**单个 HTML 文件**丢到任意静态服务器就能用
- 流式回复(边生成边显示)、发图自动压缩上传、亮暗双主题跟随系统
- 改一行刷新就生效,移动端调试成本低

## ③ 聊天后端:441 行 Node 原生

- 不用 `npm install`,直接 `node server.mjs` 就能跑
- SSE 流式对话 + 多模态(图片直喂模型)
- 内容寻址图床:上传按内容哈希存,自动去重
- 可选长期记忆:用 markdown 卡片做跨对话记忆,纯文件、可读可改、方便备份

## 说明

- 全部 **MIT 许可**,随便用、随便改
- 定位是**侧载自用**(不上架应用商店):想要「自己的服务自己用」的体验,这套正合适
- 所有个人标识(域名、密钥、账号)在开源前都已替换成占位符,各目录 README 写明要改哪几处
