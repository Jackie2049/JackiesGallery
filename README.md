# JackiesGallery

> Jackie2049 的对外作品/报告聚合站。
>
> 🌐 在线访问：<https://jackie2049.github.io/JackiesGallery/>

## 概述

JackiesGallery 把 Jackie2049 各项目的作品/报告聚合为一个纯静态站点：每份展品是单个 HTML 文件，内联全部 CSS/JS，**无构建、无外部依赖、无后端**。URL 即路径，可直链分享，托管于 GitHub Pages。

## 自动发布机制

站点使用 GitHub Pages 的 **Deploy from branch（main）** 模式：**推送 `main` 分支即触发 Pages 自动重建**，无需任何手动步骤。

## 目录结构

```
JackiesGallery/
├── index.html           # 顶层聚合入口（EXPERIMENTS 数组登记展品）
├── docs/
│   └── design-guide.md  # 设计规范（单一事实源）
└── <作品名>/
    └── index.html       # 每份展品 = 单文件自包含 HTML
```

## 添加一份新展品

1. 新建目录 `<作品名>/`，放一个自包含的 `index.html`（内联 CSS/JS，零外链）；
2. 在顶层 `index.html` 的 `EXPERIMENTS` 数组登记一条（标题 + 描述 + 链接 + 日期）；
3. 推送 `main`，GitHub Pages 自动更新，无需其他操作。

## 本地预览

```bash
git clone https://github.com/Jackie2049/JackiesGallery.git
cd JackiesGallery
python3 -m http.server 8000
# 浏览器打开 http://localhost:8000
```
