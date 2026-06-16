# Hi, I'm 刘贤宇 👋

江苏大学计算机科学与技术专业学术型硕士在读，预计 2028 届毕业。我的求职方向是 **AI 应用开发 / RAG & Agent 工程化 / 全栈偏 AI 应用开发**。

本科阶段就读于江苏大学智能科学与技术专业，研究生期间主要参与课题组企业横向项目开发，围绕苏州、扬州、镇江等地企业的真实业务需求，完成过 AI 问答系统、商户经营管理平台、体育俱乐部管理系统等项目实践。

相比单纯学习技术栈，我更关注如何把 AI 能力、前后端系统、数据库、中间件、部署监控和业务流程结合起来，真正落地到可使用、可维护、可交付的业务系统中。

目前我的论文已完成初稿，主要实验已经完成，课题阶段性收敛，后续时间安排较稳定。希望进一步进入真实业务团队，系统学习和实践主流的 Agent、RAG、Tool Calling、AI Workflow 等 AI 应用开发方向。当前可投入连续 **6-12 个月实习**，并能够按照全职节奏参与项目开发。

## About Me

* 🎓 江苏大学计算机科学与技术学术型硕士在读，本科为智能科学与技术专业
* 🤖 关注 RAG、Agent Workflow、Tool Calling、Prompt Engineering 和 AI 应用工程化
* 🧩 具备前端、后端、数据库、缓存、接口联调、部署监控等完整项目实践经验
* 🏢 研究生期间参与多个企业横向项目，具备面向真实业务需求进行开发和交付的经验
* 🚀 熟悉 Docker / Docker Compose / Nginx / Linux 等部署与工程化工具
* 📊 了解 Langfuse、Prometheus、Grafana 等观测与监控工具
* 💡 当前希望在 AI 应用开发、RAG/Agent 开发、全栈偏 AI 应用方向继续深入

## What I Focus On

除了完成项目功能本身，我更关注 AI 应用在真实业务中的工程化落地：

* 如何将企业内部资料、产品文档和业务规则整理成可检索、可追溯的 RAG 知识库
* 如何设计 Agent 工具调用流程，让模型能够调用推荐、库存、订单、支付、认证等业务接口
* 如何通过 Prompt 约束、检索参数调优、兜底策略和评测集提升 AI 回复稳定性
* 如何接入 Langfuse / Prometheus / Grafana 等工具，观察模型调用、接口状态、Token 消耗和系统性能
* 如何使用 Docker Compose、Nginx、Redis、MySQL、Elasticsearch 等组件完成项目部署与交付
* 如何在支付、退款、认证回调等业务场景中处理状态一致性、幂等控制和异常补偿
* 如何将 AI 应用与传统业务系统结合，而不是只停留在 Demo 或单轮问答层面

## Tech Stack

### AI Application

RAGFlow, LangChain, LangGraph, LangSmith, Langfuse, Embedding, RAG, Agent Workflow, Tool Calling, Function Calling, Prompt Engineering

### Backend

Python, FastAPI, Flask, Java, Spring Boot, MyBatis-Plus, RESTful API, Sa-Token, Knife4j

### Frontend

Vue3, TypeScript, Vite, Element Plus, Tailwind CSS, uni-app, unibest, ECharts

### Database & Middleware

MySQL, PostgreSQL, Redis, Elasticsearch, MinIO, pgvector

### Deployment & Observability

Linux, Shell, Docker, Docker Compose, Nginx, Prometheus, Grafana

## Repository Notice

部分项目来源于课题组企业横向项目，代码主要托管在组内私有 Gitee 仓库中，涉及企业业务数据、交付资料、接口配置和部署环境，暂不公开完整源码。

当前 GitHub 主要用于展示个人技术栈、项目经历、脱敏后的项目说明、工程实践总结和可公开的学习 / 实验代码。对于企业项目，我会在不暴露敏感信息的前提下，整理项目背景、技术架构、核心实现思路、问题排查记录和个人负责内容。

部分可公开内容已进行脱敏处理，移除了 API Key、数据库配置、企业资料、部署敏感信息和私有接口信息。

## Featured Projects

以下项目为本人在课题组横向项目和个人工程实践中的代表性经历。由于部分项目涉及企业合作与交付资料，完整源码暂不公开，仅展示脱敏后的项目背景、技术栈、核心实现和个人负责内容。

### 扬州茶博园 RAG + Agent 智能平台

面向茶园销售与客服场景，基于 RAGFlow 搭建 RAG + Agent 智能问答系统，接入 DeepSeek API 与本地 Ollama 模型，支持茶叶知识问答、产品推荐、价格库存查询、销售话术生成、冲泡建议和健康风险边界控制。

项目亮点：

* 基于 RAGFlow 构建茶园业务知识库，完成 Excel 资料导入、文档解析、Chunk 切分、Embedding 向量化和 Elasticsearch 检索配置
* 调优 TopN、TopK、相似度阈值、向量权重等检索参数，并开启引用返回机制，提升知识召回稳定性与回答可追溯性
* 接入 Open WebUI 管理的本地 Ollama 模型，配置本地推理模型与 Embedding 模型，并修复 RAGFlow 调用 Ollama Chat 接口的兼容问题
* 在 RAGFlow Agent 中编排 HTTP 工具调用流程，实现产品推荐、价格库存、冲泡建议、售后政策、健康风险等业务意图识别
* 接入 Langfuse 记录 Prompt、工具返回 JSON、模型输出、Token 消耗和响应延迟，用于排查回复异常、工具结果未引用、成本和性能问题
* 设计业务评测集，优化工具路由、字段抽取和兜底策略，提升问答系统稳定性和可控性

涉及能力：

* RAG 知识库构建
* Agent Workflow 编排
* HTTP Tool Calling
* 本地模型接入
* Prompt 约束与兜底策略
* Langfuse 可观测性
* Docker Compose 部署

### 我的圈子商户经营管理平台

面向本地生活商户经营场景，参与建设商户后台管理端与后端服务，支持商户入驻、资质认证、店铺管理、商品管理、订单管理、资金流水、经营统计、消息通知和收款二维码等业务流程。

项目亮点：

* 基于 Vue3 + Vite + Element Plus 搭建商户管理端，完成店铺、商品、订单、资金流水、经营统计和通知中心等核心模块
* 接入微信支付 V3 JSAPI，完成预下单、支付参数签名、订单查询、退款申请、退款查询和支付 / 退款回调解析
* 设计支付与退款主动补查任务，结合 Redis 分布式锁和 Lua 脚本避免多实例重复对账，提升支付状态同步可靠性
* 接入阿里云实人认证，结合 Redis 一次性 callback token、Lua 原子消费和 WebSocket 实时推送，实现认证回调校验、重复消费控制与认证结果实时通知

涉及能力：

* 商户后台管理系统开发
* 微信支付 V3 接入
* 支付 / 退款回调处理
* 主动补查与异常补偿
* Redis 分布式锁
* Lua 原子操作
* WebSocket 实时通知
* 阿里云实人认证

### 鹰速体育系统

面向体育俱乐部会员运营场景，参与建设后台管理端、微信小程序端与后端服务，支持会员管理、体测成绩、积分商城、会员卡管理、活动报名、数据统计和系统监控告警。

项目亮点：

* 基于 Vue3 + TypeScript + Vite + Element Plus 搭建后台管理端，完成会员管理、体测管理、积分商城、会员卡管理、活动课程管理和数据看板等模块
* 封装 Axios 请求、Token 注入、401 登录失效处理、路由守卫和页面级接口联调逻辑，统一后台管理端接口调用与权限访问流程
* 基于 Spring Boot + MyBatis-Plus 实现活动管理模块，完成活动新增、编辑、分页查询、报名管理、签到 / 取消报名和活动统计等接口
* 参与 uni-app / unibest 小程序端开发，完成会员信息、会员卡信息、积分记录、活动记录等个人中心功能
* 使用 Docker 部署后端服务与监控组件，接入 Prometheus + Grafana，实现服务状态、接口指标和资源使用情况的可视化监控

涉及能力：

* 后台管理系统开发
* 微信小程序开发
* RESTful API 设计
* 登录鉴权与权限访问
* 前后端联调
* Docker 部署
* Prometheus / Grafana 监控

## Research & Project Experience

研究生期间，我主要在课题组参与企业横向项目开发，项目覆盖 AI 问答、企业管理后台、微信小程序、商户支付、认证回调、数据统计和系统监控等方向。这些项目让我更熟悉真实业务开发中的需求拆解、接口设计、前后端联调、异常处理、系统部署和交付流程。

在项目开发过程中，我不仅关注功能是否能够完成，也会关注：

* 业务流程是否闭环
* 接口设计是否清晰
* 异常情况是否有兜底
* 支付 / 认证等回调场景是否具备幂等控制
* 系统是否便于部署和维护
* AI 回复结果是否可观测、可评估、可优化

目前我正在进一步学习和实践主流 AI Agent 技术方向，包括：

* Agent 状态管理与工作流编排
* RAG 检索增强生成与知识库优化
* Tool Calling / Function Calling 工具调用机制
* 多轮对话中的上下文管理与记忆机制
* AI 应用的可观测性、评测集设计和效果优化
* AI 应用与传统业务系统的结合方式

## Competition Experience

* 第十八届全国大学生交通运输科技大赛二等奖
* 第十五届大学生服务外包创新创业大赛二等奖
* 第七届全国高校智能交通创新与创业大赛三等奖
* 第十七届大学生服务外包创新创业大赛二等奖

## Current Goal

我希望寻找一份 AI 应用开发、RAG/Agent 开发或全栈偏 AI 应用方向的实习机会，在真实业务场景中继续提升工程能力。

当前可投入情况：

* 可连续实习 6-12 个月
* 可按全职节奏参与项目开发
* 课题论文已完成初稿，主要实验已完成，后续时间安排较稳定
* 对 AI Agent、RAG、工具调用、AI Workflow 和工程化部署方向有持续学习和实践意愿

## Contact

* Email: [1677837750@qq.com](mailto:1677837750@qq.com)
* GitHub: https://github.com/lxy123hh
