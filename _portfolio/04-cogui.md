---
title: "CoGUI · 人机协同的移动端 GUI 自动化"
excerpt: "在 AndroidWorld 任务集上比较无介入、高层介入、低层介入、混合介入四种人机协同模式的执行框架，支持多模拟器并行与断点续跑。<br/><span class='muted'>A human-in-the-loop framework comparing four intervention modes on AndroidWorld.</span><br/><a href='https://github.com/likelikec/CoGUI'>github.com/likelikec/CoGUI</a>"
collection: portfolio
permalink: /projects/cogui/
order: 4
---

研究的核心是把**人工介入**放进 agent 的执行链路里，并量化它到底换来了什么。

- **四种介入模式**：无介入 / 高层介入（给方向）/ 低层介入（纠动作）/ 混合介入，同一套链路横向对比。
- **任务集管理**：按任务名、任务族、序号、正则筛选 AndroidWorld 任务，自动跳过已完成任务，失败或中断后可续跑。
- **并行执行**：支持多台 Android Emulator 同时跑，默认内置 A/B/C 三个设备槽位。
- **可观察**：前端状态页实时展示任务描述、截图、规划、动作、反思、点击坐标与人工输入。
- **结构化产出**：可直接统计成功率、运行时长、执行步数、介入次数与失败原因。

**技术栈**：Python · AndroidWorld · Android Emulator · OpenAI-compatible API（如 DashScope）