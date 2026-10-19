---
title: "AI4arXiv · 论文情报聚合"
excerpt: "每个工作日自动抓取 arXiv「系统 / 软件工程 / 安全」方向的新论文与修订，按关键词、LLM 相关性、历史反馈打分分档；高价值论文生成五段式精读与经程序核验的原文证据。<br/><span class='muted'>A zero-server arXiv digest pipeline: fetch, score, deep-read, verify evidence, publish.</span><br/><a href='https://github.com/likelikec/ai4arxiv'>github.com/likelikec/ai4arxiv</a>"
collection: portfolio
permalink: /projects/ai4arxiv/
order: 6
---

把「追论文」这件事做成一条可无人值守的流水线。

- **抓取与打分**：arXiv API 拉取 cs.SE / cs.CR 等方向新论文与 v2/v3 修订，结合关键词、LLM 相关性和历史反馈打分。
- **分档推荐**：「今日必读 / 值得关注 / 其余归档」，避免信息淹没。
- **精读与核验**：高价值论文生成五段式精读、兴趣问答、写作手法分析，以及**经程序核验的原文证据**（不靠模型自己背书）。
- **零服务器**：全流程跑在 GitHub Actions 免费额度内，数据以每日 JSON 存进仓库，无需数据库；发布成功后才发精简邮件。
- **有反馈闭环**：GitHub Pages Dashboard 支持收藏、已读、不感兴趣和「多推荐此类」。

**技术栈**：Python · arXiv API · LLM · GitHub Actions · GitHub Pages