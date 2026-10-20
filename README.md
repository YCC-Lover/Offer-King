<div align="center">

<img src="docs/images/00-brand.png" width="88" height="88" alt="Offer King 皇冠与求职记录品牌图标">

# Offer King

### 把投递进度记清楚，把 Offer 选择想明白。

一个为个人求职准备的本地助手：跟进面试、少抄招聘资料、比较公司与待遇，再算清到手工资和生活预算。

**本机保存 · 无需应用账号 · AI 可选 · 中／英／日／韩界面**

[简体中文](README.md) · [English](docs/i18n/en/README.md) · [日本語](docs/i18n/ja/README.md) · [한국어](docs/i18n/ko/README.md)

**[↓ Windows 2.5.4](https://github.com/YCC-Lover/Offer-King/releases/download/v2.5.4/Offer-King-Setup-2.5.4.exe)**　·　**[↓ 安卓试用 APK](https://github.com/YCC-Lover/Offer-King/releases/download/v2.5.4/Offer-King-2.5.4-android-trial.apk)**　·　[下载与校验](docs/DOWNLOAD.md)　·　[文档中心](docs/README.md)

[下载与版本](#下载与版本) · [快速开始](#快速开始) · [主要功能](#符合你的求职节奏) · [界面预览](#界面预览) · [AI 配置](#ai-配置) · [常见问题](#常见问题) · [反馈](#反馈与参与)

</div>

> [!IMPORTANT]
> **2.5.4 是候选试用版（Pre-release），不是已验收正式版。** Windows 未正式签名；安卓使用 Debug 开发测试签名。真实 Windows 首装／覆盖／卸载、安卓真机安装／覆盖／使用尚未验收。升级先导出备份，签名冲突不要直接卸载，不要关闭安全防护。[已测与未测事项](docs/RELEASE-2.5.4.md#已验证与尚未验收)

## 下载与版本

| 你的设备 | 下载 2.5.4 | 试用边界 |
| --- | --- | --- |
| Windows 10 / 11 x64 | [Windows 安装包 .exe](https://github.com/YCC-Lover/Offer-King/releases/download/v2.5.4/Offer-King-Setup-2.5.4.exe) | 未正式数字签名（NotSigned）；NSIS 安装包 |
| Android | [安卓试用包 .apk](https://github.com/YCC-Lover/Offer-King/releases/download/v2.5.4/Offer-King-2.5.4-android-trial.apk) | Debug 签名；手机实际兼容性待验收 |

[固定候选发布页](https://github.com/YCC-Lover/Offer-King/releases/tag/v2.5.4) · [文件校验清单](https://github.com/YCC-Lover/Offer-King/releases/download/v2.5.4/SHA256SUMS.txt) · [可离线阅读的指南](https://github.com/YCC-Lover/Offer-King/releases/download/v2.5.4/START-HERE.md)

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

语言截图来自 2.3.0 打包候选程序，使用合成资料并阻断外网。公司与岗位保持原文；切换界面语言不会翻译用户内容。所有图片均标注真实来源版本，**不冒充 2.5.4 或安卓安装实拍**。

## 2.5.4：试用更清楚，Windows 更新有入口

- **Windows 与安卓候选包：** 关于页明确“小范围试用版”，分别说明签名和未验收边界。
- **Windows 新版提醒：** 使用期间每天最多自动检查一次，可关闭、忽略或手动检查；只打开官方发布页，不自动下载或安装。
- **保留现有日常工具：** 四语界面、识别录入、待办、公司风险与排行、Offer 比较、工资试算、预算和备份。[本版完整说明](docs/RELEASE-2.5.4.md) · [版本历史](CHANGELOG.md)

2.4.0 及更早公开用户需先手动升级一次，发布 Release 不会给旧 App 自动加功能。安卓 Debug 包不作为正式自动升级资产推荐；构建成功不等于手机验收通过。

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

Windows 2.5.4 有前台版本检查，发现适配版本后打开官方发布页，仍需自行备份、下载与安装。旧 2.4.0 及更早版本先手动升一次；安卓 Debug 不作为正式升级渠道。也可在 GitHub Watch 中只订阅 Releases，但 GitHub 通知不等于 App 内推送。

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

本仓库提供下载、文档和反馈渠道。**Offer King 为闭源软件，应用源码不在本仓库公开。** 当前候选 2.5.4；文档更新：2026-10-20。
