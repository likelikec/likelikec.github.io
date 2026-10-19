---
title: "WebGUIAgent · 轻量 Web GUI Agent"
excerpt: "接收网页任务 JSON，用 Playwright 驱动 Chromium，通过多角色模型链路观察、规划、定位、执行并校验，最终产出可复盘的测试报告与逐步运行产物。<br/><span class='muted'>A lightweight web GUI agent with a multi-role model chain and replayable run artifacts.</span><br/><a href='https://github.com/likelikec/WebGUIAgent'>github.com/likelikec/WebGUIAgent</a>"
collection: portfolio
order: 2
---

面向本地网页的 GUI 自动化：业务流程冒烟测试、演示系统端到端验证、以及上线前的人工可审计自动化检查。

- **多角色链路**：Observation → Reflector → Planner → Grounder → 浏览器动作执行 → 下一次观察 → Verifier。
- **元素定位与动作执行**：由 Grounder 把高层计划落到具体可交互元素上，再交给 Playwright 执行。
- **可复盘**：每个任务都有逐步运行产物和结构化测试报告，便于人工核查 agent 的判断依据。
- **定位清晰**：不包含训练、benchmark 或 WebArena 逻辑，专注做可用的执行与报告层。

**技术栈**：Python · Playwright Chromium · 多角色 LLM 链路