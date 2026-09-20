# Hongtan Liu / Olando · 项目作品集

我关注把具体需求做成可以使用、交付和持续维护的产品：从业务流程与数据处理，到 Web 应用、桌面客户端与 AI 应用探索。

[GitHub](https://github.com/Olandooooes) · [产品门户](https://xingo.fun)

## 独立工程案例

从业务问题、本人职责、技术取舍、关键实现、验证和交付边界展开：

- [OfferPath：Web 工作流、附件与 AI 简历迭代](cases/offerpath.md)
- [BitBubble：桌面交互、跨设备状态与发布维护](cases/bitbubble.md)
- [Aque：离线图片修复与 Windows 交付](cases/aque.md)
- [我的回想录：微信小程序与网站版本管理](cases/memoir.md)
- [Codex History Sync Plus：公开源码诊断恢复工具](cases/history-sync.md)

## 先看这三个项目

| 项目 | 解决的问题 | 工程重点 | 入口 |
| --- | --- | --- | --- |
| OfferPath | 岗位信息、投递状态和后续行动分散 | React / TypeScript、服务端 API、登录、数据同步、导入导出 | [在线产品](https://offerpath.xingo.fun) |
| BitBubble | 桌宠陪伴缺少人与人之间的互动 | Electron、实时连接、跨设备状态、Windows 安装包交付 | [项目与下载](https://github.com/Olandooooes/BitBubble-releases) |
| Codex History Sync Plus | 配置变化后本地对话或项目记录难以找回 | Python / PowerShell、状态诊断、备份、dry-run、恢复流程 | [公开源码](https://github.com/Olandooooes/codex-history-sync-plus) |

## OfferPath：从求职流程到完整 Web 产品

**场景：** 求职信息散落在招聘网站和表格里，投递进度、面试安排与下一步行动难以保持一致。

**产品路径：** 录入或导入岗位 → 管理阶段与活动 → 安排跟进和面试 → 查看漏斗与日程 → 导出记录。

**实现：** React / TypeScript 前端，Clerk 登录，Cloudflare Workers API 与 D1 数据存储；包含本地缓存、跨设备同步、重复检测、日历导出和提醒功能。

**值得讨论的工程问题：**

- 不同账号的本地数据如何隔离，首次登录时如何处理已有记录。
- 网络失败后如何重试，如何避免已删除记录在同步后重新出现。
- 如何把阶段变化、历史活动与下一步行动组织成可持续使用的工作流。

**体验建议：** 使用虚构公司和岗位建立记录，修改阶段与下一步，刷新后检查记录，再试导出。请勿在公开演示中使用真实求职隐私。

**范围：** 产品源码保持私有。AI 简历相关能力仍在迭代，本作品集不将未完成真实模型验收的功能写成已验证成果，也不声称已有商业收入或规模化用户。

## BitBubble：桌面交互与实时社交

**场景：** 将单机桌宠扩展成朋友之间的轻量互动入口。

**产品路径：** 创建桌宠 → 添加好友 → 派宠物串门 → 对话或传递纸条 → 返回并保留回忆。

**实现重点：** Electron 桌面窗口、鼠标穿透和管理界面，WebSocket 连接与重连，以及两端设备的访问状态协调。通过 Windows 安装包、校验文件、Release 与 Issues 完成交付和反馈闭环。

**演示重点：** 两台设备完成一次完整串门；解释断线恢复、窗口状态与打包环境问题如何定位。

[官网](https://bitbubble.xingo.fun/) · [发布与项目说明](https://github.com/Olandooooes/BitBubble-releases)

公开发布仓库不等于开源源码。Windows 为公开正式版，macOS 不作为已发布能力展示。

## Aque / 净像工坊：离线图片局部修复

**场景：** 对自有或已获授权图片中的污点、划痕和小面积遮挡进行局部修复。

**实现与交付：** Python 桌面应用、离线操作流程、Windows 安装包、独立官网与文件校验。用相同输入展示处理前后差异，同时保留原图并说明效果边界。

[官网](https://aque.xingo.fun) · [项目与下载](https://github.com/Olandooooes/Aque-releases)

## 我的回想录：微信小程序与产品交付

以微信小程序为产品入口，配套独立官网、隐私说明、版本归档和反馈。工程上将网站部署、小程序发布和源码版本追溯分别管理，避免网站更新误伤已有服务。

[官网](https://yearrings.xingo.fun) · [版本与反馈](https://github.com/Olandooooes/Xingo-releases)

在微信搜索「我的回想录」。源码归档标签不代表已经核验的微信审核版本。

## Codex History Sync Plus：在开源项目上解决具体问题

基于 [GODGOD126/codex-history-sync-tool](https://github.com/GODGOD126/codex-history-sync-tool) 扩展，保留原作者署名和 MIT 许可证。扩展重点是项目记录、线程归属、索引缺失与新版状态格式下的诊断和恢复。

仓库包含状态检查、dry-run、备份和恢复说明，以及测试运行入口。它处理本地记录，不提供跨云端账号同步，也不能恢复已被物理删除的会话。

[源码、运行说明与测试入口](https://github.com/Olandooooes/codex-history-sync-plus)

## 如何评估这些项目

- **产品体验：** 从每个项目的公开官网或发布入口开始。
- **代码阅读：** 公开源码项目可直接阅读；闭源产品通过演示与设计说明沟通，不以发布仓库代替源码证据。
- **工程讨论：** 重点讨论需求取舍、状态管理、错误处理、部署、版本追溯与验证方式。
- **事实边界：** 未公开用户数据、雇主内部系统或客户材料；未用未经核验的用户量、收入或测试结果包装项目。

*本页整理于 2026-09-20。项目状态以对应仓库和当前产品为准。*
