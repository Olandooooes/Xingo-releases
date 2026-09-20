# Codex History Sync Plus · 可检查、可回退的本地恢复工具

[← 作品集首页](../PORTFOLIO.md) · [公开源码](https://github.com/Olandooooes/codex-history-sync-plus)

> 开源扩展项目。基于 [GODGOD126/codex-history-sync-tool](https://github.com/GODGOD126/codex-history-sync-tool)，保留原作者署名、MIT License 与 NOTICE；不将上游全部能力算作本人原创。

## 问题与扩展范围

配置变化后，本地会话可能仍在数据库中，却没有出现在项目或侧边栏里。原工具处理 provider / model 变化后的历史同步；Plus 扩展关注项目记录、线程归属、索引缺失和新版状态格式。

我的贡献范围围绕这些项目恢复问题展开，同时复用上游的同步与备份能力。它只处理本地状态，不同步不同云端账号，也不能恢复已被物理删除的会话内容。

## 实现与技术

工具使用 Python、PowerShell，涉及 SQLite 状态库与 JSON / JSONL 索引。项目恢复实现将过程拆成读取现状、生成计划、显示摘要和应用计划：

```text
当前状态 + 可选备份
  → 归一化路径并读取线程
  → 生成项目与归属恢复计划
  → 默认 dry-run 检查
  → 显式 apply 前检查客户端进程
  → 备份后写入状态
```

路径处理需要应对中文目录、Windows 长路径和旧路径型项目顺序；项目存在与线程可见不是同一件事，需要同时处理项目定义、线程分配与索引。

## 关键设计

- **先计划再写入：** 默认 dry-run，让用户看到将发生的恢复；不是启动脚本就立即修改全部状态。
- **写入前检查运行状态：** 应用计划时检测客户端进程，避免在客户端正在写入时同时修改。
- **保留回退材料：** 使用上游数据库备份能力，另存项目状态备份。
- **不擅自取消归档：** 只有显式选择时，才恢复全归档项目；不批量改动用户主动归档的其他任务。
- **范围有限：** 不覆盖认证和配置文件，不能保证兼容未来所有内部格式变化。

## 验证与交付

仓库公开测试入口、运行说明、备份与恢复步骤，并提供 Windows GUI；项目恢复的新增能力当前主要通过命令行使用。本次阅读了 README 和项目恢复源码，没有在用户真实状态目录执行恢复或重新运行测试。

评估者可先读 [恢复实现](https://github.com/Olandooooes/codex-history-sync-plus/blob/main/project_recovery.py)，再查看 [测试目录](https://github.com/Olandooooes/codex-history-sync-plus/tree/main/tests)。验证时应使用独立样例和备份，不把“脚本返回成功”当作客户端显示已正确恢复。

## 维护与后续

工具价值在于把“历史消失”的表象拆成可检查的本地状态问题，并提供有边界的恢复步骤。后续需要持续维护不同状态格式的兼容测试；当前没有恢复成功率或使用人数的量化结论。

[MIT License](https://github.com/Olandooooes/codex-history-sync-plus/blob/main/LICENSE) · [来源与署名 NOTICE](https://github.com/Olandooooes/codex-history-sync-plus/blob/main/NOTICE)
