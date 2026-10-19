# likelikec.github.io

个人主页，基于 [Academic Pages](https://github.com/academicpages/academicpages.github.io) 模板（Jekyll + GitHub Pages 内置构建）。

线上地址：**https://likelikec.github.io** — 推到 `master` 分支后自动重建，通常 1 分钟内生效。

## 先改这三处

| 想改什么 | 改哪个文件 |
| --- | --- |
| 名字、单位、邮箱、学术主页链接 | `_config.yml` 里的 `title` / `name` / `author:` 段 |
| 首页自我介绍（中英双语）、研究方向 | `_pages/about.md` |
| 顶部导航（加/删栏目） | `_data/navigation.yml` |

`_config.yml` 和 `_pages/about.md` 里所有 `【…】` 和 `# TODO` 都是等着你替换的占位符。

## 加一个项目

在 `_portfolio/` 下新建 md，`order` 决定排序：

```yaml
---
title: "项目名 · 一句话定位"
excerpt: "中文一句话。<br/><span class='muted'>English one-liner.</span><br/><a href='https://github.com/likelikec/repo'>github.com/likelikec/repo</a>"
collection: portfolio
order: 8
---

正文写亮点，支持 Markdown。
```

## 加一篇论文

见 `_pages/publications.html` 顶部的注释示例（`_publications/` 目录下新建 md，`category` 取 `conferences` / `manuscripts` / `books`）。

## 本地预览（可选）

需要 Ruby 3.x：

```bash
bundle install
bundle exec jekyll serve -l -H 0.0.0.0
# 打开 http://localhost:4000
```

不想装 Ruby 也可以直接推上去看线上效果。

## 目录说明

```text
_config.yml        站点与作者配置（主要改这里）
_data/navigation.yml  顶部导航
_pages/            独立页面：about（首页）、projects、publications、404、sitemap
_portfolio/        项目卡片
_publications/     论文条目（目前为空，待补）
_sass/ _includes/ _layouts/ assets/   模板样式与结构，一般不用动
```