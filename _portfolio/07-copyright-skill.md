---
title: "软著材料生成 Skill"
excerpt: "从真实软件项目生成并校验中国计算机软件著作权登记材料（代码鉴别材料、申请表信息、用户手册、软件设计说明书），流程内设分阶段人工确认。<br/><span class='muted'>An agent skill that drafts and validates Chinese software copyright registration materials from a real codebase.</span><br/><a href='https://github.com/likelikec/software-copyright-materials-skill'>github.com/likelikec/software-copyright-materials-skill</a>"
collection: portfolio
permalink: /projects/copyright-skill/
order: 7
---

- **读项目再写材料**：材料由模型阅读真实代码后撰写，脚本只负责排版、校验与归档，避免套模板生成空话。
- **分阶段确认**：缺少必要输入时停止并提问，而不是按缺省值硬生成。
- **产出**：鉴别材料、申请表信息、五章用户手册与软件设计说明书，输出可复核的 DOCX。
- **边界明确**：只覆盖软件著作权（R11），不适用于专利、商标及非软件类作品登记。

**技术栈**：Python · Agent Skill · DOCX