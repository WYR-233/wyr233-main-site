---
title: Android 壳(网页变 App)
slug: webview-shell
description: 把网页装进一个真正的 App —— 独立图标、返回键、相册相机、长连接推送
date: 2026-09-14
weight: 3
icon: /img/proj_app_phone.webp
tags: [Android, WebView, 推送, 开源]
links:
  - title: GitHub
    website: https://github.com/WYR-233/webview-shell
  - title: Gitee
    website: https://gitee.com/wyr233/webview-shell
---

## 目标

让自己搭的网页服务,变成手机上一个**真正的 App**:独立图标、全屏无地址栏、能调相册相机、**关屏也能收到消息推送**。整套东西零第三方依赖,全部可自托管。

## 有意思的技术点

**自己做推送,不依赖厂商通道。** 手写 RFC6455 WebSocket 长连接,配上前台服务保活——国产 ROM(小米 / 华为 / vivo / 联想)的保活设置都在文档里写了引导。

**Android 15 适配。** 前台服务类型选错当天就废,键盘避让、返回键与页面抽屉打架这些坑,都踩过一遍。

**WebView 的真实案例。** 某些 WebView 不保存 cookie、页面缓存不刷新——文档里都有对应处理。

## 定位

侧载自用,不上架应用商店。想要「自己的服务自己用」的体验,这套正合适。

## 说明

- MIT 许可,随便用、随便改
- 所有个人标识(域名、密钥、账号)在开源前都替换成占位符,各目录 README 写明要改哪几处

## 入口

[GitHub](https://github.com/WYR-233/webview-shell) / [Gitee](https://gitee.com/wyr233/webview-shell)
