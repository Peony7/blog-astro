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

本站由 GitHub Actions 自动部署到 GitHub Pages：
https://peony7.github.io/blog-astro/

推送到 `main` 分支后会自动构建发布，也可以手动触发：
GitHub → Actions → Deploy to GitHub Pages → Run workflow。

本地手动发布（备用）：

```bash
npm run deploy
```
