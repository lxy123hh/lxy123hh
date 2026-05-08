# 个人 GitHub 主页

欢迎访问我的 GitHub 页面！这里是我学习和实践前端开发、Java 与 Python 后端开发、全栈开发、运维以及人工智能的地方。在这个页面，你将看到我在这些领域的项目代码。

## 关于我

你好，我是 [lxy]，目前正在深入学习并实践以下技术：

- **前端开发**：我正在掌握 HTML、CSS、JavaScript 和前端框架（Vue）来构建动态和响应式的网页应用。
- **Java 后端开发**：学习如何使用 Java 构建健壮的后端系统，了解 Spring 框架、RESTful API、数据库设计等内容。
- **Python 后端开发**：我正在通过 Python 编写后端应用，深入学习 Django、Flask 等框架，探索如何构建高效的服务器端逻辑。
- **全栈开发**：通过结合前端与后端技术，学习如何实现完整的应用架构和功能实现。
- **运维**：探索 DevOps 和系统运维，使用工具如 Docker、Kubernetes 等，了解 CI/CD 流程和云计算服务。
- **人工智能**：学习使用机器学习和深度学习框架（PyTorch）进行人工智能方面的应用。

## 项目

### 1. 个人网站:lxy123.online
* **技术栈**：**Flask**, **HTML**, **CSS**, **JavaScript**, **Vue.js**, **Element UI**, **MySQL**, **Redis**, **Gunicorn**, **Nginx**, **Prometheus**
* **项目描述**：本项目是一个基于 Flask 的个人博客网站，首页提供发布文章、评论和点赞等基本功能；同时，集成了 YOLO 深度学习模型进行图像识别，支持图像上传与实时目标检测；用户还可以通过爬虫功能查询实时天气，并展示可视化天气数据；支持文件上传与下载功能。地图功能
* **前端开发**：使用 HTML, CSS, JavaScript 开发博客页面，结合 Vue.js 和 Element UI 实现动态效果和响应式布局。
* **后端开发**：基于 Flask 实现业务逻辑，使用 MySQL 进行数据存储，通过 Redis 提升数据访问性能。项目采用 Gunicorn 作为 WSGI 服务器，确保高效的请求处理。
* **云服务器部署**：部署于阿里云服务器，使用 Nginx 进行反向代理和负载均衡，确保网站的高可用性和安全性。
* **监控与报警**：集成 Prometheus 与Grafana监控系统，实时监控服务器状态，使用 AlertManager 和 SMTP 进行异常报警，保障系统稳定运行。


### 2. 个人笔记:https://lxy123hh.vercel.app （需要梯子）
* **技术栈**：**HTML**, **CSS**, **JavaScript**, **VitePress**, **Vue.js**, **Vercel**
* **项目描述**：本项目用来记录静态资源网页。

### 3. AgentFlow：企业知识库与客服工单工作流 Agent 平台
**技术栈**：**React**, **TypeScript**, **FastAPI**, **LangGraph**, **LangChain**, **LangSmith**, **PostgreSQL**, **pgvector**, **Docker**

**职责**:设计并实现面向企业知识检索与客服售后场景的 AI Agent 本地 MVP，支持文档上传、知识库问答、订单/物流查询、客服处理建议生成、工单管理与人工审批。
* 基于 LangGraph 构建多分支 Agent 工作流，将用户请求路由至知识库问答、客服售后处理、缺订单号和普通问答分支，并通过状态管理串联检索、工具调用、业务规则判断和最终回答生成。
* 构建 RAG 知识库模块，支持 PDF / Markdown / TXT 文档解析、文本切分、Embedding 向量化、pgvector 相似度检索，并在回答中返回引用来源和片段信息。
* 使用 FastAPI 封装后端服务，设计文档、聊天、工单、审批和 Agent 执行记录等 RESTful API，基于 PostgreSQL 存储业务数据、会话记录、审批记录、工具调用日志和向量数据。
* 实现客服售后工作流，基于 mock 订单、物流和工单数据模拟业务工具调用，并对高金额退款、已签收退款等高风险场景生成pending approval，避免 Agent 直接执行敏感动作。
* 集成 AgentRun 和 ToolCallLog 记录 Agent 执行轨迹，支持查看意图识别结果、工具调用输入输出、审批状态、RAG 引用和最终回答，便于调试和问题定位。
* 接入 LangSmith 对 LangGraph 执行链路进行可选 trace，辅助观察 Agent 节点执行、工具调用过程和工作流状态流转。
* 使用 React + TypeScript 构建前端管理界面，实现文档上传、分页、删除、chunks 查看、聊天问答、引用展示、工具调用记录、工单筛选、审批详情和人工审批操作。
* 使用 Docker Compose 编排 PostgreSQL、后端和前端服务，并编写 README、架构说明、Agent 工作流图和本地启动文档，提升项目可复现性。

### 4. 鹰速体育系统
**技术栈**：**Vue3**, **TypeScript**, **Vite**, **Element Plus**, **TailwindCSS**, **uni-app**,**unibest**,**Spring Boot**,**MyBatis-Plus**, **MySQL**, **Redis**, **Sa-Token**, **Docker**, **Prometheus**, **Grafana**

**职责**:面向体育俱乐部会员运营场景，参与建设后台管理端、微信小程序端与后端服务，支持会员管理、体测成绩、积分商城、会员卡管理、活动报名、数据统计和系统监控告警。
* 独立负责后台管理系统的原型设计与前端开发，完成登录鉴权、会员管理、体测管理、积分商城、会员卡管理、活动课程管理和数据看板等核心模块。
* 基于 Vue3 + TypeScript + Vite + Element Plus 搭建管理端前端工程，封装 Axios 请求、Token 注入、401 登录失效处理、路由守卫和页面级接口联调逻辑。
* 负责后端活动管理模块开发，基于 Spring Boot + MyBatis-Plus 实现活动新增、编辑、分页查询、报名管理、签到/取消报名和活动统计等接口。
* 参与微信小程序端开发，负责“我的”页面，实现会员信息展示、会员卡信息、积分记录、活动记录等个人中心相关功能。
* 使用 Sa-Token + Redis 配合完成登录态管理与接口鉴权联调，保障后台管理端和小程序端的权限访问流程。
* 使用 Docker 部署后端服务与监控组件，接入 Prometheus + Grafana，实现服务状态、接口指标和资源使用情况的可视化监控与异常告警。
* 参与前后端联调与业务流程设计，打通会员、活动、积分、会员卡等核心业务在后台端、小程序端和后端服务之间的数据流转。




## 技术栈

- **前端**：HTML, CSS, JavaScript, Vue3, Vite
- **后端**：Java, Spring Boot, Python, Django, Flask，MySql
- **运维工具**：Docker, Kubernetes, GitLab CI/CD
- **人工智能**： 深度学习（pytorch），机器学习，自然语言处理，图像识别，数据挖掘，数据分析

## 联系我

如果你对我的项目感兴趣，或者想交流技术，可以通过以下方式联系我：

- qq：1677837750
- 邮箱：1677837750@qq.com

感谢访问我的 GitHub 页面！我会持续更新和分享我的学习进展和项目成果。
