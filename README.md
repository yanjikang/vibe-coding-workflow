# Vibe Coding 全链路实战开发流程图

> 多窗口上下文隔离 · Rules 动态驱动 · 3 次熔断闭环

![Vibe Coding 全链路实战开发流程图](flowchart.png)

**[👉 点击打开交互式展示页](https://yanjikang.github.io/vibe-coding-workflow/)**（支持缩放 / 平移 / 分层查看）

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

- **[📖 深度讲解指南 GUIDE.md](GUIDE.md)**：一句话心法、熔断四步、Rules 反哺、SOP 检查清单、五分钟上手示例
- **[🌐 在线展示页](https://yanjikang.github.io/vibe-coding-workflow/)**：交互式流程图，支持缩放、平移、分层查看
- **源文件**：[Vibe-Coding-Workflow.drawio](Vibe-Coding-Workflow.drawio)，用 [app.diagrams.net](https://app.diagrams.net/) 或 draw.io Desktop 打开即可编辑

## 配套模板（templates/）

工作流的"记忆"全靠四份本地文档承载，新项目直接复制起步：

| 模板 | 作用 | 对应步骤 |
|------|------|----------|
| [plan.md](templates/plan.md) | 开发计划：产品概述、技术栈锁定、里程碑拆解、完成定义 | Step 03 |
| [docs.md](templates/docs.md) | 开发文档：架构、目录约定、数据模型、接口契约、ADR | Step 03 |
| [rules.md](templates/rules.md) | 项目规范：技术栈约束 + 严禁事项（踩坑沉淀区） | Step 04/06，持续反哺 |
| [progress.md](templates/progress.md) | 进度交接：已完成/待办/技术债/熔断记录 | Step 15 |

## 文件说明

```
├── index.html                  # 展示页（内嵌 draw.io viewer，无需构建）
├── GUIDE.md                    # 深度讲解：心法 / 熔断 / Rules 反哺 / SOP / 上手示例
├── flowchart.png               # 流程图预览图（README 展示用，2x 高清导出）
├── Vibe-Coding-Workflow.drawio # draw.io 源文件（1920×1080 黑色主题）
├── templates/                  # 四大核心资产模板（plan / docs / rules / progress）
└── README.md
```

## License

图表内容仅供学习交流，欢迎注明出处后转载。
