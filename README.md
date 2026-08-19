# Peony7 的博客

基于 [Astro](https://astro.build) 构建的个人博客，由 Hexo 迁移而来。

## 本地开发

需要 Node.js >= 22。

```bash
npm install
npm run dev       # 启动开发服务器
npm run build     # 构建静态站点到 dist/
npm run preview   # 本地预览构建产物
```

## 内容管理

文章放在 `src/content/blog/`，支持 Markdown（`.md`）。每篇文章的 frontmatter：

```yaml
---
title: "文章标题"
description: "文章摘要"
pubDate: 2017-05-12
category: "CSS"
tags: ["css"]
---
```

图片放在 `public/images/` 目录，文章中通过 `/images/...` 引用。

## 部署

本站使用 `gh-pages` 分支部署到 GitHub Pages：
https://peony7.github.io/blog-astro/

发布新版本：

```bash
npm run deploy
```
