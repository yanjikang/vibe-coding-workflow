# Vibe Coding 全链路实战开发流程图

> 多窗口上下文隔离 · Rules 动态驱动 · 3 次熔断闭环

一套经过实战验证的 AI 辅助开发（Vibe Coding）完整工作流，覆盖从"一个想法"到"正式上线"的全部 21 个步骤，按 5 个阶段组织：

| 阶段 | 名称 | 要点 |
|------|------|------|
| STAGE 01 | 需求对齐与基建生成 | 对话窗口 1：聊透产品形态、锁定主流技术栈、产出 plan.md / docs.md / 通用 Rules |
| STAGE 02 | 项目规范定制与 MVP 开发 | 对话窗口 2（净空上下文）：定制项目专属 Rules，开启任务模式，视觉先行构建 MVP |
| STAGE 03 | 测试验证、修 Bug 循环与 3 次熔断 | 运行预览 → 有 Bug 则常规排错并反哺 Rules；同一 Bug 超过 3 次触发熔断：Git 回滚 + 新窗口止损 |
| STAGE 04 | 存档交接与多窗口功能迭代 | Git Commit 安全存档 → 更新 progress.md → 结构瘦身重构 → 新窗口 N 接力下一功能 |
| STAGE 05 | 全局联调与收尾上线 | 清理调试日志与测试数据 → 打包构建 → 部署上线，完成闭环 |

## 跨窗口四大核心资产

窗口随时可以新建，"记忆"永远留在本地文档里：

- **plan.md / docs.md** — 全局蓝图（任务拆解 + 数据/接口架构）
- **rules.md** — 防踩坑编码规范，随高频错误持续反哺
- **progress.md** — 跨窗口接力棒，新窗口读取即可续接进度
- **Git Commit** — 每个验证通过的版本都是可随时回滚的安全锚点

## 查看方式

- **在线展示页**（推荐）：启用本仓库的 GitHub Pages 后访问 `index.html`，流程图可直接在浏览器中缩放、分层查看
- **源文件**：[Vibe-Coding-Workflow.drawio](Vibe-Coding-Workflow.drawio)，用 [app.diagrams.net](https://app.diagrams.net/) 或 draw.io Desktop 打开即可编辑
- **本地预览**：直接双击 `index.html` 用浏览器打开

## 文件说明

```
├── index.html                  # 展示页（内嵌 draw.io viewer，无需构建）
├── Vibe-Coding-Workflow.drawio # draw.io 源文件（1920×1080 黑色主题）
└── README.md
```

## License

图表内容仅供学习交流，欢迎注明出处后转载。
