# 麦扑科技（OMAPS）

[中文](#麦扑科技omaps) · [English](#english) · [官网](https://www.omaps.cn) · [技术博客](https://blog.omaps.cn)

**户外媒体（OOH）点位数字化管理平台**

OMAPS 覆盖点位资源、订单投放、派单上刊、完工报告全流程，PC 管理后台与移动端现场作业双端协同，把点位台账、排期、投放与结算放进同一套系统。

## 产品能力

| 模块 | 内容 |
|---|---|
| 点位与地图 | 经纬度落位、空位按区域/规格/档期高亮、框选片区算容量、点位包成组上地图、实景照片挂到点位 |
| 投放流程 | 选点 → 锁点（排期锁定防撞单）→ 派单上刊 → 完工报告（自动生成 PPT 并打包原图） |
| 业务中台 | 客户档案、商机跟进、销售与采购合同、统一审核中心、经营报表、作业量与考勤 |
| 财务结算 | 请款与逾期标记、到款与划拨、发票、提成核算、客户对账、会计期间与结转 |
| 移动端作业 | 微信小程序 / 独立 App：任务接收、GPS 签到、拍照水印、断网补传 |
| AI Copilot | 基于 AgentScope 的销售助理：查可投点位、按预算拆组合、生成投放方案、口述拜访转记录 |

## 工程

- **后端**：Java + Spring Boot 多模块，CQRS 命令通道、多租户数据隔离、对象级访问控制
- **前端**：Vue 3 + TypeScript
- **开放接入**：OpenAPI 接口与 MCP 协议，AI 客户端可直接调用点位与排期查询
- **部署形态**：SaaS（多租户）与本地部署（数据不出内网）

## 能力边界

先把不适配的说清楚，省一轮试错：

- **以静态平面媒体为主**（大牌、候车亭、灯箱、道闸、墙体）。LED 数字屏只做排期与档期占位，**不做播放内容推送、屏体控制、播放日志回传，也不含 SSP / DSP 程序化交易对接**。
- **不做 AI 图像质检**：照片是否错刊、遮挡、翻拍，由时间地点水印、GPS 定位与人工复核判定。
- **提成为单级比例**（划拨金额 × 比例）；多级阶梯、跨项目拆账、集团合并报表属定制评估范围。

## 技术博客

工程实践、架构与治理文档发在 [blog.omaps.cn](https://blog.omaps.cn)：

- [AI 不可替代的：面向客户的主营业务流程与落地引擎](https://blog.omaps.cn/post/customer-centric-workflow-engine/)（2026-11-15）
- [企业 AI 落地：企业上下文、内部 FDE 与场景闸门](https://blog.omaps.cn/post/enterprise-ai-landing/)（2026-11-12）
- [AI 原生研发：产物链、门禁与度量](https://blog.omaps.cn/post/ai-native-sdlc-gates/)（2026-11-12）
- [API 业务访问与完整性风险清单](https://blog.omaps.cn/post/api-access-integrity-risks/)（2026-11-12）

## 联系我们

- 官网 / 预约演示：<https://www.omaps.cn>
- 商务邮箱：sales@omaps.cn
- 地址：广州市天河区金穗路 1 号邦华广场

---

<a id="english"></a>

# OMAPS

[中文](#麦扑科技omaps) · **English** · [Website](https://www.omaps.cn) · [Tech Blog](https://blog.omaps.cn)

**Digital management platform for out-of-home (OOH) media inventory**

OMAPS covers the full OOH campaign lifecycle — inventory, order placement, dispatch and billboard posting, completion reporting — with a PC admin console and a mobile field-work app working in tandem, bringing inventory ledgers, scheduling, campaign execution and billing into a single system.

## Product Capabilities

| Module | Scope |
|---|---|
| Inventory & Map | Geocoded inventory placement, slot availability highlighted by region/spec/availability window, area selection with capacity estimation, inventory bundles grouped on map, site photos attached to inventory records |
| Campaign Workflow | Site selection → slot locking (schedule locks prevent double-booking) → dispatch & posting → completion report (auto-generated PPT with original photos packaged) |
| Business Middle Platform | Client profiles, opportunity tracking, sales & procurement contracts, unified approval center, business reports, workload & attendance |
| Financial Settlement | Payment requests & overdue flags, receipts & allocation, invoices, commission calculation, client reconciliation, accounting periods & carry-forward |
| Mobile Field Work | WeChat mini program / standalone app: task receipt, GPS check-in, photo watermarking, offline capture with later sync |
| AI Copilot | AgentScope-based sales assistant: find available inventory, build packages by budget, generate campaign proposals, turn spoken visit notes into records |

## Engineering

- **Backend**: Java + Spring Boot multi-module, CQRS command pipeline, multi-tenant data isolation, object-level access control
- **Frontend**: Vue 3 + TypeScript
- **Open Integration**: OpenAPI and MCP protocol — AI clients can query inventory and schedules directly
- **Deployment**: SaaS (multi-tenant) or on-premise (data stays inside the intranet)

## Scope Boundaries

Where we don't fit, stated up front to save everyone a round of evaluation:

- **Static OOH media first** (billboards, bus shelters, light boxes, gate barriers, wall panels). LED digital screens are supported for scheduling and availability placeholders only — **no content push, no screen control, no play-log collection, and no SSP/DSP programmatic trading integration**.
- **No AI photo QA**: whether a photo shows a mis-post, occlusion, or a re-shot board is judged by time/location watermarks, GPS positioning, and human review.
- **Single-tier commission** (allocated amount × rate); multi-tier ladders, cross-project splitting, and consolidated group reporting fall under custom evaluation.

## Tech Blog

Engineering practice, architecture and governance notes live at [blog.omaps.cn](https://blog.omaps.cn):

- [What AI Cannot Replace: Customer-Facing Core Business Workflows and the Delivery Engine](https://blog.omaps.cn/en/post/customer-centric-workflow-engine/) (2026-11-15)
- [Enterprise AI Adoption: Organizational Context, Internal FDEs, and Scenario Gates](https://blog.omaps.cn/en/post/enterprise-ai-landing/) (2026-11-12)
- [AI-Native Engineering: Artifact Chains, Gates, and Metrics](https://blog.omaps.cn/en/post/ai-native-sdlc-gates/) (2026-11-12)
- [API Access and Integrity Risk Catalog](https://blog.omaps.cn/en/post/api-access-integrity-risks/) (2026-11-12)

## Contact

- Website / book a demo: <https://www.omaps.cn>
- Sales: sales@omaps.cn
- Address: Banghua Plaza, 1 Jinsui Road, Tianhe District, Guangzhou, China
