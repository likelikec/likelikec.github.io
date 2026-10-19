---
title: "PC-Agent · 桌面 GUI 测试 Agent"
excerpt: "纯视觉的桌面 GUI 自动化测试执行 agent：整屏截图 → 视觉语言模型规划与元素定位 → 真实鼠标键盘事件 → 可读测试报告（HTML / Excel / 截图轨迹 / GIF）。<br/><span class='muted'>Vision-only desktop GUI test agent that drives a native app and emits auditable reports.</span><br/><a href='https://github.com/likelikec/PC-Agent'>github.com/likelikec/PC-Agent</a>"
collection: portfolio
order: 1
---

目标场景是在受控的 Linux X11 桌面（例如 VMware 虚拟机）里，对着一个被测程序（如 C++ 工控 / SCADA 软件）按给定测试步骤自动操作，并对照「预期结果」给出 **Pass / Fail / Unknown** 判定。

- **纯视觉执行**：不依赖控件树或 accessibility 接口，只对整屏截图做规划与元素定位（默认 Qwen3-VL）。
- **真实输入**：执行侧用 `mss` 截图 + `pyautogui` 驱动鼠标键盘，操作的是原生桌面程序而非浏览器。
- **可审计产物**：每步留下截图轨迹、动作记录与判定理由，最终汇总成 HTML + Excel 报告和 GIF。
- **来源**：由一个 Web GUI Agent 改造而来，保留了原有多角色循环与产物结构，只替换执行层。

**技术栈**：Python · 视觉语言模型 · mss · pyautogui · Linux X11