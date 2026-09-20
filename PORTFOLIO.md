# 刘红潭 / Hongtan Liu · 工程作品集

**AI 应用 · 全栈开发 · FDE / 技术交付**  
从业务需求出发，完成软件实现、验证交付与持续维护。

| **[工作项目 · 企业需求落地](#work-projects)** | **[个人项目 · 产品开发与交付](#personal-projects)** |
| :--- | :--- |
| **智采**：采购部门实际使用的内部工具<br>**链析**：规则匹配、历史归档与数据处理<br>**企业系统**：Web 改造、Flutter 移动端维护 | **OfferPath**：已上线的求职管理 Web 产品<br>**BitBubble**：Windows 社交桌宠，黑客松二等奖¹<br>**开源工具**：可直接阅读的诊断与恢复实现 |
| 重点：**业务理解、需求响应、数据处理、维护** | 重点：**产品设计、工程实现、发布、迭代** |
| **端与架构：** Web（B/S）· Windows 桌面（C/S）· Flutter iOS / Android | **端与架构：** Web（B/S）· 桌面客户端（C/S）· 微信小程序 · 离线单机工具 |

[GitHub](https://github.com/Olandooooes) · [产品门户](https://xingo.fun) · [OfferPath 在线体验](https://offerpath.xingo.fun) · [BitBubble 官网](https://bitbubble.xingo.fun/)

<a id="work-projects"></a>

## 工作项目 · 企业需求落地

**富士医疗技术服务（上海）有限公司｜2024.07 至今**  
早期 PACS 医院远程支持，后转内部系统开发维护。以下为脱敏案例，点击项目名查看职责、实现、验证与交付细节。

| 项目 | 我做了什么 | 重点成果 / 工程证据 |
| --- | --- | --- |
| **[智采 · 采购管理工具](cases/zhicai.md)** | 整理历史 Excel、结构化建库；开发查询、录入、看板和供应商模块<br>**AI 辅助：** Gemini、ChatGPT、GitHub Copilot、Cursor | **采购部门实际使用**；需求到业务工具的落地 |
| **[链析 · 报价规则处理](cases/lianxi.md)** | **Windows 桌面 · C/S**；Python / PySide6 / SQL Server，规则匹配与归档<br>**AI 辅助：** Gemini、ChatGPT、GitHub Copilot、Cursor | **可追溯的历史任务**；处理失败与导出状态控制 |
| **[企业 Web / 移动端系统](cases/enterprise-systems.md)** | **Web · B/S：** ASP.NET MVC 审批改造<br>**iOS / Android · C/S：** Flutter 恢复与维护<br>**AI 辅助：** ChatGPT、Codex | **遗留系统接管与迭代**；在途数据迁移、真机与模拟验证分层 |
| **[销售报表自动化](cases/sales-reporting.md)** | Salesforce → Python / SQL → Power BI，覆盖 6 条产品线 | 月度整理流程自述 **约 6 人时 → 20 分钟**² |
| **[设备手册 AI 问答](cases/manual-qa.md)** | FastAPI 检索、百炼 / DeepSeek 接入、引用与原页图片预览 | **答案可回查来源**；适配 Windows 部署环境 |
| **[影刀 RPA · 招投标信息采集](cases/rpa.md)** | 使用**影刀 RPA**串联自动登录、批量检索、资料与招投标信息采集、结构化导出 | 自述覆盖 **400 余竞品目标**；异常与结果核验细节待补证 |

**项目性质：** 企业内部软件案例，源码与业务数据不公开。[软件著作权记录与归属边界](cases/software-rights.md)。开发贡献与企业软件权利归属分别说明。

<a id="personal-projects"></a>

## 个人项目 · 产品开发与交付

**独立产品开发｜Web · Windows 桌面 · 微信小程序 · 开源扩展**  
从产品流程到实现、发布和维护；闭源产品提供体验入口，开源项目提供可检查代码。  
**主要 AI 辅助开发工具：ChatGPT、Codex**。用于需求梳理、代码理解、实现与调试；由我检查结果、验证流程并负责交付。

| 项目 | 我做了什么 | 重点成果 / 体验入口 |
| --- | --- | --- |
| **[OfferPath · 求职流程管理](cases/offerpath.md)** | **Web · B/S**；React / TypeScript、Clerk、Workers / D1；岗位管理、同步与附件 | **已上线 Web 产品** · [在线体验](https://offerpath.xingo.fun) |
| **[BitBubble · 社交桌宠](cases/bitbubble.md)** | **Windows 桌面 · C/S**；Electron / WebSocket；跨电脑串门、状态与安装包 | **外滩黑客松二等奖¹** · [下载与版本](https://github.com/Olandooooes/BitBubble-releases) |
| **[Aque · 净像工坊](cases/aque.md)** | **Windows 桌面 · 离线单机**；Python / OpenCV；局部修复、预览与安装包 | **离线桌面产品** · [官网](https://aque.xingo.fun) · [下载](https://github.com/Olandooooes/Aque-releases) |
| **[我的回想录](cases/memoir.md)** | **微信小程序客户端 + 服务端 API**，配套 **Web 官网（B/S）**；隐私说明与版本追溯 | **小程序产品交付** · [官网与入口](https://yearrings.xingo.fun) |
| **[Codex History Sync Plus](cases/history-sync.md)** | **本地 CLI / Windows GUI**；在上游基础上扩展索引诊断、dry-run、备份与恢复 | **公开源码** · [实现与测试](https://github.com/Olandooooes/codex-history-sync-plus) |

¹ 奖项来自本人提供的经历；相关内容 5 万余播放是传播数据，不是用户数。  
² 耗时来自本人工作记录；新旧任务的计时范围仍待进一步核实。

<details>
<summary>背景、验证范围与开发方式</summary>

上海健康医学院 · 数据科学与大数据技术本科 · 2020.09–2024.06。职业经历自 2024.07 起，转岗月份尚未核实，不将总工龄等同于全栈开发年限。

案例分别标明工作自述、代码核查、既有验收记录和公开发布。模拟测试不等于生产验收；Flutter 维护不等于独立原生双端开发；规则匹配不等于训练预测模型。OfferPath 的真实模型调用和 Resume Matcher 生产集成尚未完成验证。

AI 辅助开发工具按项目列出；它们与产品运行时调用的百炼 / DeepSeek API 分开说明。B/S 指浏览器访问服务端；C/S 指安装或宿主中的客户端访问服务端。离线单机工具单独标明，不套用联网架构。由我明确需求、检查生成结果、验证流程并承担交付责任。企业案例不附内部源码、客户或供应商明细、真实报价、生产配置、凭据或用户数据。图示均为流程概括。

</details>

*更新于 2026-09-20。详细状态以各案例和公开 Release 为准。*
