# JackiesGallery

> 🌐 Jackie2049 的小画廊，展示可视化结果、分析报告等材料。访问链接：<https://jackie2049.github.io/JackiesGallery/>

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
