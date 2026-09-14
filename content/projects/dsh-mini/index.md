---
title: dsh-mini 极简发行包
slug: dsh-mini
description: 一个 exe 双击就能用的 AI 助手 —— 单文件、免安装、无需管理员权限
date: 2026-09-14
weight: 1
icon: /img/proj_dshmini.webp
tags: [DeepSeek Harness, Windows, 开源]
links:
  - title: 官网
    website: https://dshmini.wyr233.com
  - title: GitHub
    website: https://github.com/WYR-233/dsh-mini
  - title: Gitee
    website: https://gitee.com/wyr233/dsh-mini
---

## 它解决什么问题

想用 AI 助手,却要先装 Node、配环境变量、开终端敲命令——**第一步就劝退**。

dsh-mini 把整套流程压缩成一个 exe:**下载 → 双击 → 用**。适合不想折腾环境的人,也适合公司电脑、学校电脑这类不方便装软件的环境。

## 亮点

- **单文件打包**:运行时 + 服务 + 界面全塞进一个 exe
- **自带 Node 运行时**:不污染系统环境,删文件夹就等于卸载干净
- **不需要管理员权限**:装在自己的用户目录里
- **全中文向导**:安装、升级、卸载全程有指引
- **升级不丢数据**:配置与对话记录独立存放

## 技术要点

把 Node 服务打包进 exe,启动时在临时目录展开并拉起本地服务,再由内置窗口访问;Release 由 CI 在打 tag 时自动构建,GitHub 主发 + Gitee 镜像。

## 下载

- 官网:[dshmini.wyr233.com](https://dshmini.wyr233.com)
- [GitHub Releases](https://github.com/WYR-233/dsh-mini/releases/latest) / [Gitee 镜像](https://gitee.com/wyr233/dsh-mini)

开源免费,MIT 协议。
