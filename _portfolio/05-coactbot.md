---
title: "CoactBot · 轨迹感知自我纠正的移动作业台"
excerpt: "人在回路的移动 GUI 自动化：以轨迹为单位的自我纠正机制，配合 React 工作台观察与接管 agent 的每一步。<br/><span class='muted'>Human-in-the-loop mobile GUI automation with trajectory-aware self-correction.</span><br/><a href='https://github.com/likelikec/CoactBot'>github.com/likelikec/CoactBot</a>"
collection: portfolio
permalink: /projects/coactbot/
order: 5
---

- **轨迹级纠正**：不只纠正单步动作，而是基于已走过的轨迹判断该回到哪个状态重试。
- **人在回路**：提供可观察、可接管的工作台，人能随时插入指令或修正。
- **双通道设备控制**：同时支持 ADB 与 HDC，覆盖常规 Android 设备与鸿蒙设备。
- **编排**：以 LangGraph 组织 agent 的状态机与纠正流程；前端为 React + Vite。

**状态**：Research Preview（研究预览）

**技术栈**：Python · LangGraph · React + Vite · ADB / HDC