# Product
<!-- impeccable:product-schema 1 -->
## Platform
web
## Stack
Vue 3 + Vite, Node 原生 HTTP；本地 JSON 存储。用户要求临时 Vue 项目，设计细节已委托。
## Users
需要日常处理表格数据的人。当前用户以桌面查看、体验与撰写 Agent 前端文章为目的。
## Product Purpose
批量数据处理工作台：选择数据集、创建任务、跟踪进度、处理失败、下载 CSV。
## Operating Context
仅本机临时演示；数据集为生成的示例，历史任务明确标为演示数据。后端实际处理数据并保存状态。
## Capabilities and Constraints
桌面端优先；不做手机版本；不改博客。无外部服务、账户、支付或权限管理。只采用 Vue、Vite 及官方 Vue 插件，服务端不新增依赖。
## Brand Commitments
禁止通过卡片或提示框的左侧彩色竖线强调重点。图标默认不添加，仅用于明确的操作或识别用途；不使用闪电、火箭、星光等装饰图标。专业、克制、合理的信息密度。名称“序列”为此次演示拟名。
## Evidence on Hand
本地生成数据集以及真实 API 和执行日志；没有真实商业客户、使用量或效果指标。
## Product Principles
- 操作有结果、状态可解释。
- 失败有原因和恢复入口。
- 保持用户输入，防止重复提交。
- 使用统一的表格、表单、状态与反馈语言。
