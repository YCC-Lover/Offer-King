<div align="center">

<img src="docs/images/00-brand.png" width="88" height="88" alt="Offer King 皇冠与求职记录品牌图标">

# Offer King

### 把投递进度记清楚，把 Offer 选择想明白。

一个为个人求职准备的本地助手：跟进面试、少抄招聘资料、比较公司与待遇，再算清到手工资和生活预算。

**本机保存 · 无需应用账号 · AI 可选 · 中／英／日／韩界面**

[简体中文](README.md) · [English](docs/i18n/en/README.md) · [日本語](docs/i18n/ja/README.md) · [한국어](docs/i18n/ko/README.md)

**[↓ Windows 2.6.0](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.0/Offer-King-Setup-2.6.0.exe)**　·　**[↓ 安卓 2.6.1 试用 APK](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.1/Offer-King-2.6.1-android-trial.apk)**　·　[下载与校验](docs/DOWNLOAD.md)　·　[文档中心](docs/README.md)

[下载与版本](#下载与版本) · [快速开始](#快速开始) · [主要功能](#符合你的求职节奏) · [界面预览](#界面预览) · [AI 配置](#ai-配置) · [常见问题](#常见问题) · [反馈](#反馈与参与)

</div>

> [!IMPORTANT]
> **Android 2.6.1 / Windows 2.6.0 均为候选试用版（Pre-release）。** Windows 未正式签名；安卓使用 Debug 开发测试签名。真实 Windows 首装／覆盖／卸载、安卓真机首装／覆盖／使用及升级后 AI 解密尚未验收。升级先导出备份，签名冲突不要直接卸载，不要关闭安全防护。[安卓已测与未测](docs/RELEASE-2.6.1.md#已验证与尚未验收) · [Windows 原范围](docs/RELEASE-2.6.0.md#已验证与尚未验收)

## 下载与版本

| 你的设备 | 当前固定下载 | 试用边界 |
| --- | --- | --- |
| Windows 10 / 11 x64 | [Windows 安装包 .exe](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.0/Offer-King-Setup-2.6.0.exe) | 未正式数字签名（NotSigned）；NSIS 安装包 |
| Android | [安卓 2.6.1 试用包 .apk](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.1/Offer-King-2.6.1-android-trial.apk) | Debug 签名；真机首装／覆盖未验收 |

[安卓 2.6.1 发布页](https://github.com/YCC-Lover/Offer-King/releases/tag/v2.6.1) · [安卓校验与指南](docs/DOWNLOAD.md) · [Windows 2.6.0 发布页](https://github.com/YCC-Lover/Offer-King/releases/tag/v2.6.0)

**下载不需要 GitHub 登录，也不需要开发工具。** 不设试用期限，不人为限制本地功能；AI 服务可能收费。系统要求、升级顺序及 SHA-256 见[下载中心](docs/DOWNLOAD.md)。

暂不提供 macOS、iOS 或 Linux 安装包。GitHub 的 Latest 可能仍指旧版本，请使用上面的固定链接；自动生成的 `Source code` ZIP 只有公开文档，**不是安装包，也不是 App 源码**。

## 快速开始

1. **先试一条虚构投递。** 下载、校验后，新增公司与岗位；可以粘贴招聘文字，先在本机识别，再核对公司、岗位、城市与阶段。无需先配 AI。
2. **给下一步留个位置。** 设置事项和时间，明确保存，再关闭重开确认记录仍在。首页与全部待办帮助你跟进；它们不是关闭 App 后运行的系统闹钟。
3. **资料齐了再比较。** 后续补充薪酬、个人评分和城市预算；定期导出 JSON，附件原文件另外保管。

已有记录？先在旧版导出备份，再更新，最后核对资料。[完整上手教程](docs/QUICKSTART.md) · [候选试用检查顺序](docs/DOWNLOAD.md#试用时先检查这五件事)

每位朋友从自己的本机空数据开始。手机与电脑**各自保存，不自动同步**；不要把个人数据目录、备份或密钥一并分享。

## 符合你的求职节奏

| 想解决的事 | Offer King 能帮你做什么 |
| --- | --- |
| 多家公司同时投，下一步容易忘 | 阶段看板、独立岗位流程、下一事项与全部待办；同一公司可关联多个岗位 |
| 招聘介绍太长，不想逐项手抄 | 本机粘贴识别明确字段，勾选后填空白；也可选用模型提取或联网补全 |
| 两份待遇难取舍 | 常态年包与首年总包分开看，Offer 对比与双 Offer PK 保留个人权重 |
| 想知道公司是否适合自己 | 公司库、带来源的风险评估及六类个人公司排行；缺资料不硬排前三 |
| 税前工资和换城市预算算不清 | 本地到手工资试算、自选缴费基数与比例，再按自己的房租、通勤和生活预算估算储蓄 |
| 担心看不清或忘了备份 | 浅／深色主题、90%–125% 字号、独立滚动、JSON 导出与本机备份 |

本地记录、比较、文字识别和工资试算不需要 AI。风险与排行是辅助判断，不是企业客观评级；工资试算面向中国大陆人民币场景，不是报税或 HR 实发承诺，城市预算也不是实时市场均价。[功能与计算口径](docs/FEATURES.md)

## 界面预览

### 投递跟进：每家公司走到哪一步，一眼找到

<a href="docs/FEATURES.md#1-投递跟进下一步始终有着落"><img src="docs/images/03-board.png" alt="求职看板：岗位按面试阶段排列，各列独立滚动，均为虚构演示资料"></a>

拖动卡片或选择阶段，打开详情查看流程。下一事项可按逾期、今天、未来七天、以后和待安排时间查看。

*上图来自 2.0.0 实际 Windows 应用的合成演示，不是当前安卓实拍。[截图来源与版本](docs/images/README.md)*

### 到手工资：先核对参数，再看实际参考价值

![2.4.0 到手工资页面：示例月薪、城市、自选缴费基数和比例，以及年度明细](docs/images/20-payroll.png)

从岗位带入人民币月薪，调整自己的城市、基数与比例，查看个人缴费、个税与 12 个月到手估算；不改原岗位工资。城市名称不代表已自动匹配当地政策。

*上图来自 2.4.0 实际程序的独立合成环境；示例参数不是工资单、城市统一政策或报税验收。*

<details>
<summary><strong>少抄资料：查看本机招聘文字识别</strong></summary>

![2.4.0 本机招聘文字识别：原文、证据和勾选预览，不覆盖已有输入](docs/images/21-local-capture.png)

先核对证据，再填勾选的空白项。无需网络、模型或搜索密钥；完整原文不进入恢复草稿和备份，只有采纳字段可保存。截图来自 2.4.0 合成演示。

</details>

<details>
<summary><strong>比较机会：查看双 Offer PK</strong></summary>

![2.0.0 双 Offer PK：雷达图展示维度差异，条形图展示个人权重下的综合分](docs/images/09-pk-charts.png)

得分反映你填写的资料与权重，不代表企业客观排名。截图为 2.0.0 合成演示。[比较口径](docs/FEATURES.md#2-待遇决策把数字和个人偏好分清楚)

</details>

[英语界面](docs/images/17-english-ui.png) · [日本語](docs/images/18-japanese-ui.png) · [한국어](docs/images/19-korean-ui.png) · [城市预算、公司库和更多界面](docs/FEATURES.md)

语言截图来自 2.3.0 打包候选程序，使用合成资料并阻断外网。公司与岗位保持原文；切换界面语言不会翻译用户内容。所有图片均标注真实来源版本，**不冒充 2.6.0 或安卓安装实拍**。

## 安卓 2.6.1：在 App 内发现后续新版

修复试用 APK 的版本识别，支持前台自动提醒、手动检查，以及打开对应官方发布页下载；也改善深色模式更新卡片的可读性。**安卓 2.6.0 及更早试用用户须先手动覆盖升级到 2.6.1 一次。** 之后在“帮助与关于 → 应用更新”允许候选版提醒，才能发现后续更高版本，不会自动下载或安装。

沿用 2.6.0 的应用身份与开发签名，覆盖更新设计为保留记录和 AI 配置。先导出备份，再选择“更新”，不要先卸载、清除数据或重置 AI；JSON 不含密钥和附件文件。**真机首装、覆盖安装及升级后 AI 密钥解密尚未验收。** [本版完整说明](docs/RELEASE-2.6.1.md) · [覆盖升级步骤](docs/DOWNLOAD.md#已有记录先备份再升级)

## 2.6.0：找得快、看得全、跟得上

- **快速查找：** 点击顶部查找按钮或按 `Ctrl+K`，搜索本机公司、岗位、城市、技能、阶段和页面；支持多关键词与键盘选择，不调用 AI。
- **看板／列表随时切换：** 按阶段推进，或每页 30 条集中浏览；固定表头和身份列，长列表可独立横向、纵向滚动。
- **留下常用筛选：** 组合阶段、优先级、城市、办公方式、收藏和待办条件，最多保存 12 个命名视图，下次直接使用。
- **更轻松地安排下一步：** 从首页、看板或全部待办打开快速跟进，选择明天、下周或自定义时间，明确保存后写入流程，不改求职阶段。
- **首页与详情更好读：** 待办优先、长表单按需展开；优化小窗口、手机、大字号及输入法操作。[本版完整说明](docs/RELEASE-2.6.0.md) · [操作指南](docs/QUICKSTART.md#260-日常效率工具) · [版本历史](CHANGELOG.md)

这些日常工具继续保留。AI 提供商和费用策略沿用原配置；常用视图只保存在当前设备，不进入求职 JSON 备份。Windows 当前安装包仍为 2.6.0，2.5.4 起支持前台版本提醒。安卓当前为 2.6.1，修复试用包识别；两端均需自行下载、安装，检查版本不调用 AI。

## AI 配置

**先不配置也能用。** 需要减少录入或查询资料时，再选适合自己的路线：

| 任务 | 要准备什么 | 资料怎样处理 |
| --- | --- | --- |
| 本机识别招聘文字 | 不需要模型、密钥或网络 | 按规则识别明确字段，预览后填空白 |
| 用 AI 理解已有招聘原文 | 自己的兼容岗位模型，或已准备好的本机 Ollama | 云端路线发送粘贴文字，不等于联网核实；先移除私人信息 |
| 联网补全／调研公开资料 | 对应模型与搜索能力，或已支持的原有提供商路线 | 核对来源与查询时间，采纳到草稿后明确保存 |

[从这里配置 AI →](docs/AI-SETUP.md) · [已有模型如何接入](docs/AI-SETUP.md#4-配置自己的模型) · [平台差异](docs/AI-SETUP.md#先确认你使用的平台)

安装包**没有共享 API Key**。“免费 AI 起步”需要自己的 OpenRouter／Tavily 账号和密钥，不保证永久免费；模型、搜索和测试可能消耗额度。模型连接成功不代表搜索已配置，手机的 localhost 也不是电脑。

“创建岗位后自动调研”默认关闭，主动启用后才调用。取消请求不能撤销服务商已经处理部分的计费；未知信息仍需自行核实。

## 常见问题

<details>
<summary><strong>不配置 AI、没有网络，也能管理求职吗？</strong></summary>

可以。本地记录、流程、待办、文字识别、薪酬比较、工资试算、预算和备份不依赖 AI。官网图标、版本检查及主动 AI 功能可能联网；提醒只在 App 内显示，不是后台系统闹钟。

</details>

<details>
<summary><strong>朋友会收到我的公司记录或密钥吗？</strong></summary>

不会。安装包不包含作者的求职资料、缓存或密钥，每人使用自己的本机记录和服务账户。目前无云同步或遥测。只分享安装包、指南或项目链接，不分享个人数据目录。

密钥在本机加密且不进入业务 JSON 备份；普通记录、恢复草稿和备份不是加密保险箱。Windows 附件只记录路径，安卓使用系统文档授权；附件原文件与授权不随 JSON 迁移，换设备需重新选择。[数据与隐私](docs/PRIVACY.md)

</details>

<details>
<summary><strong>为什么没有自动升级？怎样收到新版本消息？</strong></summary>

Windows 2.5.4 起已有前台版本检查，当前下载仍为 2.6.0；旧 2.4.0 及更早版本需先手动升级。安卓 2.6.1 起识别官方试用 APK，2.6.0 及更早安卓试用版需先手动覆盖一次。允许候选提醒、网络可达且存在更高版本的适配文件时，App 才会提醒并打开发布页；仍需自行备份、下载与安装。GitHub Watch 是 GitHub／邮箱通知，不是给所有旧 App 远程推送功能。

</details>

<details>
<summary><strong>能用英语、日语、韩语，或在其他系统安装吗？</strong></summary>

界面提供中／英／日／韩，在侧栏或显示设置即时切换，保留正在编辑的内容；公司名、备注、人工阶段和已有 AI 原文保持不变。语言偏好仅存在本机，不进入求职备份。

本轮只提供 Windows x64 和安卓开发候选。没有 macOS、iOS、Linux 安装包；Windows 最小窗口 1100×700 不适用于手机。[下载与平台限制](docs/DOWNLOAD.md)

</details>

[更多常见问题](docs/FAQ.md) · [文档中心](docs/README.md)

## 反馈与参与

不需要会写代码。写清**版本与系统 → 操作步骤 → 期望与实际结果**，就能帮助下一版更好用。安装、界面、AI 等补充项只在相关时填写；中／英／日／韩反馈均欢迎。

[报告问题](https://github.com/YCC-Lover/Offer-King/issues/new?template=bug_report.yml) · [功能建议](https://github.com/YCC-Lover/Offer-King/issues/new?template=feature_request.yml) · [文档／翻译纠错](https://github.com/YCC-Lover/Offer-King/issues/new?template=docs_feedback.yml) · [反馈指南](CONTRIBUTING.md)

Issues 对所有人公开。请打码，不要上传密钥、完整备份、真实附件或私人路径；潜在漏洞使用[私密安全反馈](SECURITY.md)。

觉得有帮助，可以 Star 收藏或把[项目主页](https://github.com/YCC-Lover/Offer-King)分享给求职中的朋友。不需要分享整个项目或个人数据目录。

---

[文档中心](docs/README.md) · [所有版本](https://github.com/YCC-Lover/Offer-King/releases) · [后续方向](ROADMAP.md) · [使用许可](LICENSE.md) · [第三方声明](THIRD-PARTY-NOTICES.txt)

本仓库提供下载、文档和反馈渠道。**Offer King 为闭源软件，应用源码不在本仓库公开。** 当前候选：Android 2.6.1、Windows 2.6.0；文档更新：2026-10-24。
