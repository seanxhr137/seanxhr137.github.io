# 谢和睿 · 个人博客

这是一个使用 Markdown、Jekyll、HTML 和 CSS 的静态个人博客。GitHub Actions 会在推送到 `main` 后构建并发布到 GitHub Pages；本机无需安装额外构建工具。

## 写文章

在 `_posts/` 新建 `YYYY-MM-DD-title.md`，保留文章布局和 Front Matter：

```yaml
---
layout: post
title: 文章标题
date: 2026-10-26
excerpt: 一句话摘要
tags:
  - 随笔
---
```

第二个 `---` 后写 Markdown 正文。首页从 `_posts/` 自动显示最新文章。

## 修改站点

- 站点名称、描述和时区：`_config.yml`
- 首页文案和项目：`index.html`
- 关于页：`about.md`
- 页面结构：`_layouts/`
- 配色与排版：`assets/style.css`
- GitHub Pages 自动部署：`.github/workflows/pages.yml`

## 发布

仓库的 Pages 来源设为 **GitHub Actions**。检查并提交更改后推送到 `main`，Actions 会运行 Jekyll 并部署网站。
