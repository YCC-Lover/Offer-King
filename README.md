<div align="center">

<img src="docs/images/00-brand.png" width="88" height="88" alt="Offer King 皇冠与求职记录品牌图标">

# Offer King

### 从第一条投递，到更有把握的选择。

把面试进度、薪资待遇和城市生活放在一起，选适合自己的 Offer。

**Windows 10 / 11 · x64 · 本机保存 · 无需应用账号 · AI 可选**

**[下载 2.2.0 候选试用版](https://github.com/YCC-Lover/Offer-King/releases/download/v2.2.0/Offer-King-Setup-2.2.0.exe)**　·　[安装与校验](docs/QUICKSTART.md#1-下载并安装)　·　[功能导览](docs/FEATURES.md)

[文档中心](docs/README.md) · [AI 配置指南](docs/AI-SETUP.md) · [更新记录](CHANGELOG.md) · [反馈问题](https://github.com/YCC-Lover/Offer-King/issues/new/choose)

</div>

> **试用前请知悉：** 2.2.0 是未签名的候选试用版（Pre-release），**真实干净 Windows 首装、覆盖安装和卸载尚未验收**。旧用户升级前请导出 JSON 备份，另行保管附件原文件；遇到系统拦截不要关闭安全防护。[发布说明与验证范围](docs/RELEASE-2.2.0.md)

![Offer King 首页：集中查看 Offer、面试进度和待办，图中均为合成演示资料](docs/images/01-dashboard.png)

*上图来自 2.0.0 实际应用的合成演示环境；AI 导览图来自 2.1.1 模拟响应。首次使用从自己的空白资料开始。[查看更多界面](docs/FEATURES.md) · [截图来源](docs/images/README.md)*

## 你现在想做什么？

| 你的目标 | 直接前往 |
| --- | --- |
| 先了解它是否适合自己 | [功能与界面导览](docs/FEATURES.md) |
| 下载，记录第一条投递 | [安装与图文上手](docs/QUICKSTART.md) |
| 把招聘介绍整理成字段 | [粘贴招聘原文](docs/AI-SETUP.md#新方式粘贴招聘原文)，只需岗位模型，无需搜索密钥 |
| 根据公司和岗位查询公开资料 | [AI 配置指南](docs/AI-SETUP.md)，按需要配置模型与搜索 |
| 遇到问题，或者想提建议 | [常见问题](docs/FAQ.md) · [反馈入口](CONTRIBUTING.md) |

## 跟好进度，也看清选择

**Offer King 是一款面向个人求职的 Windows 桌面应用。** 从投递、笔试、面试到 Offer，用一份本机记录串起整个过程。信息逐渐完整后，再比较待遇、城市预算和自己的偏好。

- **投递跟进：** 阶段看板、流程时间线、下一事项与五组全部待办；同一家公司关联多个岗位。
- **待遇决策：** 常态年包与首年总包分开看；保存城市生活预算，做双 Offer PK，记录评分、权重与取舍。
- **公司风险：** 维护公司共享资料，查看个人评分、排行和带来源的风险评估；保留人工判断。
- **AI 辅助：** 联网调研公开资料，或提取粘贴的招聘原文；建议先到草稿，核对后明确保存。

本地记录、看板、比较和备份无需配置 AI，也无需应用账号。资料保存在各自电脑，朋友之间不会自动同步。

[浏览功能与真实界面 →](docs/FEATURES.md)

## 2.2.0 有哪些新变化？

- **待办看全：** 逾期、今天、未来七天、以后、待安排时间集中查看，完成事项会留下流程记录。
- **决策草稿可恢复：** PK 与城市预算异常退出后可预览、恢复到表单，再核对保存。暂存容量有限，仍需定期备份。
- **招聘原文可提取：** 粘贴岗位介绍，提取有原文证据的职责、技能、薪酬等字段；建议默认不选，结果标注“未经联网核实”。
- **AI 配置可排查：** 一键检查已保存的岗位路由、模型结构化输出及搜索来源；同意费用后才发送测试请求。

[查看完整更新与已测／待测项目 →](docs/RELEASE-2.2.0.md)

## 十分钟开始使用

1. **下载并校验。** 从 [2.2.0 发布页](https://github.com/YCC-Lover/Offer-King/releases/tag/v2.2.0) 下载 `Offer-King-Setup-2.2.0.exe` 和 `SHA256.txt`，按[上手指南](docs/QUICKSTART.md#1-下载并安装)核对。无需下载源码或安装开发工具。
2. **留下第一条投递。** 填写公司、岗位和阶段，安排下一事项，明确保存。不确定的资料可以以后补。
3. **做好自己的备份。** 在“设置与备份”导出 JSON，另外保管附件原文件。有了待遇信息后，再试城市预算和 Offer PK。

下载无需 GitHub 账号；提交公开反馈需要账号。当前提供 Windows x64 安装包，没有手机、macOS 或 Linux 安装版，也没有自动更新。

GitHub 自动生成的 **Source code** 压缩包仅含本仓库文档，不能安装 App。当前候选版请使用上面的固定链接；GitHub 的 Latest 标记仍指向[上一版 2.1.1](https://github.com/YCC-Lover/Offer-King/releases/tag/v2.1.1)。

## AI 按你的需要配置

| 想完成的任务 | 需要准备 |
| --- | --- |
| 只用本地管理与比较 | 无需 AI 配置 |
| 提取已有招聘原文 | 自己的岗位模型，或已准备好模型的本机 Ollama；不要求搜索密钥 |
| 联网查公开资料 | 支持的模型与对应搜索配置；可使用免费起步预设、自定义模型或原有提供商路线 |

安装包**没有内置共享 API Key**。“免费 AI 起步”需要自己的 OpenRouter／Tavily 账号与密钥，额度和可用性取决于服务商。模型、搜索及连接检查可能消耗额度；取消不能撤销服务商已处理请求的计费。

云端原文提取会发送你粘贴的文字，请先移除敏感内容。完整原文只在窗口内存中保留，**已采纳字段及有限证据摘录可进入草稿、记录和备份**。AI 结果、风险等级和个人评分都需要自行核实。

[按步骤配置与排查 AI →](docs/AI-SETUP.md)

## 数据由你保管

记录以本机保存为主，当前没有云同步或遥测。公司官网图标和主动启用的 AI 功能可能联网；具体发送范围见[数据与隐私](docs/PRIVACY.md)。

API Key 在本机加密，不进入求职 JSON 备份。普通记录、恢复草稿和备份不是加密保险箱；附件仅保存路径，备份不包含附件文件。本机自动备份和恢复草稿也不能代替独立保管的正式备份。

## 欢迎一起改进

使用中卡住了，或发现“这里还可以更方便”，都欢迎反馈。请写清版本、操作步骤、期望和实际结果；页面问题可补充字号、主题和系统缩放。

[报告问题](https://github.com/YCC-Lover/Offer-King/issues/new?template=bug_report.yml) · [功能建议](https://github.com/YCC-Lover/Offer-King/issues/new?template=feature_request.yml) · [文档纠错](https://github.com/YCC-Lover/Offer-King/issues/new?template=docs_feedback.yml) · [私密安全反馈](SECURITY.md)

Issues 对所有人公开。请先打码，不要上传密钥、完整求职备份、真实附件或含私人路径的日志。[反馈指南](CONTRIBUTING.md)

觉得有帮助，欢迎 Star 收藏或把[项目主页](https://github.com/YCC-Lover/Offer-King)分享给求职中的朋友；想收到版本消息，可在 GitHub Watch 中订阅 Releases。

---

[文档中心](docs/README.md) · [所有版本](https://github.com/YCC-Lover/Offer-King/releases) · [后续方向](ROADMAP.md) · [使用许可](LICENSE.md) · [第三方声明](THIRD-PARTY-NOTICES.txt)

本仓库提供安装包入口、说明文档和反馈渠道。**Offer King 为闭源软件，应用源码不在本仓库公开。** 当前候选版 2.2.0；文档更新：2026-10-15。
