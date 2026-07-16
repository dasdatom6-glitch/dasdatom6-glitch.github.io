---
title: "Hello World - 博客上线了"
date: 2026-07-16
draft: false
description: "第一篇博客文章，记录博客搭建过程。"
categories: ["随笔"]
tags: ["博客", "Hugo"]
---

## 写在前面

折腾了一番，博客终于上线了。

这个博客用 [Hugo](https://gohugo.io/) + [Stack](https://github.com/CaiJimmy/hugo-theme-stack) 主题搭建，部署在 GitHub Pages 上。

## 搭建过程

### 环境准备

```bash
# 安装 Hugo (macOS)
brew install hugo

# 安装 Hugo (Linux)
sudo apt install hugo

# 或者直接下载二进制
# https://github.com/gohugoio/hugo/releases
```

### 创建站点

```bash
hugo new site my-blog
cd my-blog
git init
git submodule add https://github.com/CaiJimmy/hugo-theme-stack.git themes/hugo-theme-stack
```

### 本地预览

```bash
hugo server -D
# 访问 http://localhost:1313
```

### 部署到 GitHub Pages

1. 在 GitHub 创建仓库 `<用户名>.github.io`
2. 推送代码
3. 在仓库 Settings → Pages 中启用 GitHub Actions 部署

## 以后的计划

写一些技术笔记、安全研究、CTF 题解之类的东西。

Stay tuned. 🚀
