# 麦朴科技（XOMAPS）

[中文](#麦朴科技omaps) · [English](#english) · [官网](https://www.xomaps.com) · [技术博客](https://blog.omaps.cn)

**AI + Cloud 生态公司**

**Xomaps = 成长路径**：X 是 eXpansion（拓展、突破跃迁），O 是 Orbit（周期、闭环、蓄力轨道），Maps 是路径与进程——在一轮轮闭环沉淀之后持续向外突破拓展，这就是成长的路径。我们是一家助力成长的公司。

麦朴科技（XOMAPS）以自研软件平台为底座，围绕企业 AI 落地提供场景诊断、Agent 定制、AI 原生研发与培训、云与托管 IT 服务——既是平台厂商，也是 AI 落地的亲历者：先在自己身上完成 AI Native 转型，平台与 Agent 在真实业务中每天生产运行。中英双语服务全球客户，官网 [www.xomaps.com](https://www.xomaps.com)。

## 业务方向

| 方向 | 内容 |
|---|---|
| 行业应用 | 线下资源数字化管理平台（自研），从户外媒体（OOH）行业起家：地图选点、排期锁定、派单上刊、完工报告全流程，业务、财务与人力一体化，SaaS 与私有化双形态交付 |
| 企业 AI 落地 | 以「企业上下文 + 场景闸门」识别高价值场景，FDE 现场共创，用真实材料与真实流程验证结果 |
| Agent 定制 | 基于 AgentScope 打造业务 Agent：销售助理、知识问答、流程协同与运营分析；OpenAPI 与 MCP 接入企业自有系统 |
| AI 原生研发与培训 | 产物链、门禁与度量的工程化方法，让 AI 产出可复现、可验收；从高管认知到骨干实操的分层培训 |
| 云与托管 IT | 云架构设计与迁移、SaaS 交付与私有化部署、托管运维与持续升级 |

## 行业应用：线下资源数字化管理平台

**线下资源数字化管理平台**，覆盖点位资源、订单投放、派单上刊、完工报告全流程，并提供客户经营、协作工单、财务结算与人力考勤等中后台能力，PC 管理后台与移动端现场作业双端协同。

| 模块 | 内容 |
|---|---|
| 点位与地图 | 经纬度落位、空位按区域/规格/档期高亮、框选片区算容量、点位包成组上地图、实景照片挂到点位 |
| 投放流程 | 选点 → 锁点（排期锁定防撞单）→ 派单上刊 → 完工报告（自动生成 PPT 并打包原图）；LED 数字屏支持全量轮播清单按版本整体下发到租户自接的播控系统 |
| 客户经营 | 客户报备（撞单保护、有效期占用与到期释放）、公海池、客户跟进记录、商机跟进、销售业绩季度聚合与月环比/年同比 |
| 业务中台 | 协作工单（跨部门发起→受理→完成→关闭，SLA 超时扫描与看板）、销售与采购合同、合同变更单、提成规则配置、统一审核中心、经营报表 |
| 财务结算 | 请款与逾期标记、到款与划拨、发票、提成核算、客户对账、会计期间与结转 |
| 人力管理 | 组织架构、员工档案（入职登记、离职/调动流程）、班次模板与月度排班（排班×派单联动）、考勤打卡与月报、保险台账 |
| 移动端作业 | 微信小程序 / 独立 App：任务接收、GPS 签到、拍照水印、断网补传、考勤打卡（定位+围栏+补卡）、任务到期提醒 |
| AI Copilot | 基于 AgentScope 的销售助理：查可投点位、按预算拆组合、生成投放方案、口述拜访转记录 |

## 工程

- **后端**：Java + Spring Boot 多模块，CQRS 命令通道（60+ 资源收口）、多租户数据隔离、对象级访问控制
- **前端**：Vue 3 + TypeScript
- **开放接入**：OpenAPI 接口与 MCP 协议，AI 客户端可直接调用点位与排期查询
- **企业微信集成**：组织架构同步、打卡数据源、任务与工单通知
- **部署形态**：SaaS（多租户）与本地部署（数据不出内网）

## 能力边界

先把不适配的说清楚，省一轮试错：

- **以静态平面媒体为主**（大牌、候车亭、灯箱、道闸、墙体）。LED 数字屏走**播控衔接层**：管点位资产、档期、屏级容量校验与下发指令，投放审核通过后把全量轮播清单按版本整体下发到租户自接的播控系统（云桥 / 内网桥）；**不做播控引擎与屏体控制**，播放凭证 v1 以人工验收兜底，也**不含 SSP / DSP 程序化交易对接**。
- **不做 AI 图像质检**：照片是否错刊、遮挡、翻拍，由时间地点水印、GPS 定位与人工复核判定。
- **提成为单级比例**（划拨金额 × 比例）；多级阶梯、跨项目拆账、集团合并报表属定制评估范围。

## 技术博客

工程实践、架构与治理文档发在 [blog.omaps.cn](https://blog.omaps.cn)：

- [一个 AI 项目的困局，与 AI 无关：并发、排队与错位的三个月](https://blog.omaps.cn/post/ai-app-project-retrospective/)（2026-11-15）
- [AI 不可替代的：面向客户的主营业务流程与落地引擎](https://blog.omaps.cn/post/customer-centric-workflow-engine/)（2026-11-15）
- [IT托管服务的升级：AI时代中小企业IT的新选择](https://blog.omaps.cn/post/shared-it-ai-era/)（2026-11-14）
- [2027 年企业 IT 部门的方向：上下文厚度与研发范围重构](https://blog.omaps.cn/post/2027-ai-directions/)（2026-11-13）
- [企业 AI 落地：企业上下文、内部 FDE 与场景闸门](https://blog.omaps.cn/post/enterprise-ai-landing/)（2026-11-12）
- [AI 原生研发：产物链、门禁与度量](https://blog.omaps.cn/post/ai-native-sdlc-gates/)（2026-11-12）
- [API 业务访问与完整性风险清单](https://blog.omaps.cn/post/api-access-integrity-risks/)（2026-11-12）

## 联系我们

- 官网 / 预约咨询：<https://www.xomaps.com>
- 商务邮箱：sales@xomaps.com
- 地址：广州市天河区金穗路 1 号邦华广场

---

<a id="english"></a>

# XOMAPS Technology

[中文](#麦朴科技omaps) · **English** · [Website](https://www.xomaps.com) · [Tech Blog](https://blog.omaps.cn)

**AI + Cloud ecosystem company**

**Xomaps means growth paths**: X = eXpansion (breaking through to the next stage), O = Orbit (closing the loop and building momentum), Maps = pathways and progress. Expansion after every closed orbit — that is the path of growth. We are a company that powers growth.

XOMAPS Technology builds its own software platform and surrounds it with enterprise AI landing services: scenario diagnosis, Agent customization, AI-native engineering enablement, and cloud & managed IT — we are both a platform vendor and a hands-on AI adopter: we completed our own AI-native transformation first, with the platform and agents running in production on our real business every day, serving clients worldwide in English and Chinese via [www.xomaps.com](https://www.xomaps.com).

## Service Directions

| Direction | Scope |
|---|---|
| Industry Application | Offline resource digitalization platform (self-developed), born in the out-of-home (OOH) industry: map-based site selection, schedule locking, dispatch & posting, completion reporting, with CRM, finance and HR built in; delivered as SaaS or on-premise |
| Enterprise AI Landing | Identifying high-value scenarios through "organizational context + scenario gates", with Forward-Deployed Engineers co-creating on-site, validated against real materials and real workflows |
| Agent Customization | Business agents built on AgentScope: sales assistants, knowledge Q&A, process orchestration and operations analysis; OpenAPI and MCP integration with your own systems |
| AI-Native Engineering & Training | An artifact-chain, gate and metrics framework that makes AI output reproducible and verifiable; tiered training from executive briefings to practitioner bootcamps |
| Cloud & Managed IT | Cloud architecture design and migration, SaaS delivery and on-premise deployment, managed operations and continuous upgrades |

## Industry Application: Offline Resource Digitalization Platform

**Offline resource digitalization platform for out-of-home (OOH) media** covering the full campaign lifecycle — inventory, order placement, dispatch and posting, completion reporting — plus back-office capabilities for client operations, cross-department work orders, financial settlement and HR attendance, with a PC admin console and a mobile field-work app working in tandem.

| Module | Scope |
|---|---|
| Inventory & Map | Geocoded inventory placement, slot availability highlighted by region/spec/availability window, area selection with capacity estimation, inventory bundles grouped on map, site photos attached to inventory records |
| Campaign Workflow | Site selection → slot locking (schedule locks prevent double-booking) → dispatch & posting → completion report (auto-generated PPT with original photos packaged); LED digital screens support versioned full-manifest delivery to the tenant's own broadcast control system |
| Client Operations | Client registration (conflict protection, validity windows with release on expiry), public pool, client follow-up records, opportunity tracking, sales performance with quarterly aggregation and month-over-month / year-over-year comparison |
| Business Middle Platform | Cross-department work orders (initiate → accept → complete → close, with SLA timeout scanning and kanban), sales & procurement contracts, contract change orders, commission rule configuration, unified approval center, business reports |
| Financial Settlement | Payment requests & overdue flags, receipts & allocation, invoices, commission calculation, client reconciliation, accounting periods & carry-forward |
| Human Resources | Org structure, employee records (onboarding, offboarding & transfer workflows), shift templates & monthly scheduling (linked with dispatch), attendance check-in & monthly reports, insurance ledger |
| Mobile Field Work | WeChat mini program / standalone app: task receipt, GPS check-in, photo watermarking, offline capture with later sync, attendance check-in (location + geofence + makeup), task due reminders |
| AI Copilot | AgentScope-based sales assistant: find available inventory, build packages by budget, generate campaign proposals, turn spoken visit notes into records |

## Engineering

- **Backend**: Java + Spring Boot multi-module, CQRS command pipeline (60+ resources consolidated), multi-tenant data isolation, object-level access control
- **Frontend**: Vue 3 + TypeScript
- **Open Integration**: OpenAPI and MCP protocol — AI clients can query inventory and schedules directly
- **WeCom Integration**: org structure sync, attendance data source, task & work-order notifications
- **Delivery**: SaaS (multi-tenant) or on-premise (data stays inside the intranet)

## Scope Boundaries

Where we don't fit, stated up front to save everyone a round of evaluation:

- **Static OOH media first** (billboards, bus shelters, light boxes, gate barriers, wall panels). For LED digital screens we provide a **broadcast-control bridge layer**: inventory assets, scheduling, screen-level capacity checks, and delivery commands — once a campaign is approved, the full program manifest is pushed as a versioned whole to the tenant's own broadcast control system (cloud bridge / intranet bridge). **No broadcast engine or direct screen control** (screens and control accounts stay with the tenant); play proof in v1 relies on manual acceptance, and **no SSP/DSP programmatic trading integration**.
- **No AI photo QA**: whether a photo shows a mis-post, occlusion, or a re-shot board is judged by time/location watermarks, GPS positioning, and human review.
- **Single-tier commission** (allocated amount × rate); multi-tier ladders, cross-project splitting, and consolidated group reporting fall under custom evaluation.

## Tech Blog

Engineering practice, architecture and governance notes live at [blog.omaps.cn](https://blog.omaps.cn):

- [The Trouble with This AI Project Had Nothing to Do with AI: Concurrency, Queuing, and Three Months of Misalignment](https://blog.omaps.cn/en/post/ai-app-project-retrospective/) (2026-11-15)
- [What AI Cannot Replace: Customer-Facing Core Business Workflows and the Delivery Engine](https://blog.omaps.cn/en/post/customer-centric-workflow-engine/) (2026-11-15)
- [The Upgrade of Managed IT Services: A New Option for SMB IT in the AI Era](https://blog.omaps.cn/en/post/shared-it-ai-era/) (2026-11-14)
- [2027 Directions for Enterprise IT Teams: Context Thickness and Rethinking the Scope of Engineering](https://blog.omaps.cn/en/post/2027-ai-directions/) (2026-11-13)
- [Enterprise AI Adoption: Organizational Context, Internal FDEs, and Scenario Gates](https://blog.omaps.cn/en/post/enterprise-ai-landing/) (2026-11-12)
- [AI-Native Engineering: Artifact Chains, Gates, and Metrics](https://blog.omaps.cn/en/post/ai-native-sdlc-gates/) (2026-11-12)
- [API Access and Integrity Risk Catalog](https://blog.omaps.cn/en/post/api-access-integrity-risks/) (2026-11-12)

## Contact

- Website / book a consultation: <https://www.xomaps.com>
- Sales: sales@xomaps.com
- Address: Banghua Plaza, 1 Jinsui Road, Tianhe District, Guangzhou, China
