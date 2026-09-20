# 我的回想录 / Xingo Releases

## 产品与项目展示 / Project overview

「我的回想录」以微信小程序作为使用入口，配套独立产品官网、隐私说明、版本归档与问题反馈，围绕个人回忆记录提供产品体验。

### 工程与交付重点

- 小程序、产品官网和服务端 API 分工，网站更新与小程序发布分别管理。
- 通过源码归档和版本说明建立追溯关系，不将源码标签冒充微信审核版本。
- 将公开产品材料与私有源码、用户记录分离。
- 官网中的界面示意与真实截图明确区分，避免把设计画面当作实测证据。

### 如何体验

在微信搜索「我的回想录」；先使用虚构内容体验记录流程，再查看产品内的数据与隐私说明。具体可用功能以当前小程序为准。

**English:** My Memoir is a WeChat mini-program project with a dedicated product website, version archives and public feedback. Its delivery workflow keeps website deployment, mini-program release and source-version traceability separate.

这里是微信小程序「我的回想录」的公开版本归档与问题反馈仓库。

- 我的回想录官网：<https://yearrings.xingo.fun>
- Xingo AI 工坊：<https://xingo.fun>
- 微信进入方式：打开微信，搜索小程序 `我的回想录`
- 隐私政策：<https://yearrings.xingo.fun/privacy>
- 用户协议：<https://yearrings.xingo.fun/terms>
- 问题与建议：[提交 Issue](https://github.com/Olandooooes/Xingo-releases/issues/new/choose)

## 当前归档

`v1.0.5` 是根据私有源码提交与现有部署记录建立的首个可追溯源码归档。它不等同于未经核验的微信公众平台后台版本号；审核版本号、审核日期与上线日期在没有可靠来源时保持未知。

[查看 v1.0.5 Release](https://github.com/Olandooooes/Xingo-releases/releases/tag/v1.0.5)

2026-07-29 起，「我的回想录」的独立产品官网迁移至 `yearrings.xingo.fun`，`xingo.fun` 作为 Xingo AI 工坊与个人作品门户。已发布 Release 与追溯资产保持不可覆盖；其中保存的旧 apex 链接仍作为当时归档依据保留。

## 关于下载

这是微信小程序，不提供 Windows、macOS、Android 或 iOS 安装包。请勿从非官方渠道下载所谓“Xingo 安装包”。获得可核验的官方小程序码后，本仓库和官网才会补充扫码入口；不会使用个人微信二维码替代。

## 仓库边界

本仓库只公开：

- 版本说明与更新记录；
- 官网、隐私政策、用户协议和微信搜索入口；
- 不含秘密的源码 commit SHA 与版本追溯清单；
- 问题反馈模板；
- 经核验后可公开的小程序码或产品截图。

小程序源码与云函数源码保存在私有仓库。本仓库不包含 AppSecret、云函数密钥、Supabase service role、用户数据或构建安装包。

公开 Issue 对所有人可见。请勿粘贴原始记录、手机号、openid、验证码、密钥或其他个人敏感信息；涉及个人数据的请求请优先通过小程序内「我的 → 数据与安全 → 隐私与数据」联系微信客服。
