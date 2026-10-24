# 下载 Offer King：Android 2.6.1 / Windows 2.6.0

[简体中文](DOWNLOAD.md) · [English](i18n/en/DOWNLOAD.md) · [日本語](i18n/ja/DOWNLOAD.md) · [한국어](i18n/ko/DOWNLOAD.md)

[项目首页](../README.md) · [文档中心](README.md) · [功能导览](FEATURES.md) · [AI 配置](AI-SETUP.md)

**候选试用版（Pre-release），无需应用账号；AI 可选。** 不设试用到期时间，不人为限制本地功能。每个人从自己的本机空数据开始，设备之间不自动同步。

> Windows 未正式数字签名；安卓带开发测试签名。真实 Windows 首装、覆盖安装和卸载，以及安卓真机安装、覆盖与使用均未验收。愿意接受这些限制再试用，升级前先导出 JSON。不要关闭系统安全防护或因签名冲突直接卸载旧应用。

## 选择你的平台

| 平台 | 当前固定下载 | 大小／说明 |
| --- | --- | --- |
| Windows 10/11 x64 | [Windows 安装包 .exe](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.0/Offer-King-Setup-2.6.0.exe) | 112,107,822 字节；NotSigned；NSIS 安装包 |
| Android | [安卓 2.6.1 试用包 .apk](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.1/Offer-King-2.6.1-android-trial.apk) | 33,735,427 字节；Debug 签名；真机首装／覆盖未验收 |
| macOS / iOS / Linux | 暂无安装包 | 源码准备或另一平台编译成功，不等于已有可安装版本 |

[安卓 2.6.1 发布页](https://github.com/YCC-Lover/Offer-King/releases/tag/v2.6.1) · [安卓更新与验收范围](RELEASE-2.6.1.md) · [Windows 2.6.0 发布页](https://github.com/YCC-Lover/Offer-King/releases/tag/v2.6.0) · [Windows 原验证范围](RELEASE-2.6.0.md)

GitHub 的 Latest 可能仍指向旧正式标记；请使用本页固定链接。公开下载不要求 GitHub 登录，也不需要开发工具。`Source code` ZIP 仅是本公开仓库的文档，不是安装包或应用源码。

## 一起下载的说明与校验

- 安卓 2.6.1：[SHA256SUMS.txt](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.1/SHA256SUMS.txt)、[START-HERE.md](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.1/START-HERE.md)、[TEST-RESULTS.md](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.1/TEST-RESULTS.md)、[TEST-RESULTS.json](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.1/TEST-RESULTS.json)：本版 APK、升级和 AI 配置保留说明、实际测试范围。
- Windows 2.6.0：[校验文件](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.0/SHA256SUMS.txt)、[离线指南](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.0/START-HERE.md)、[原测试摘要](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.0/TEST-RESULTS.json)。本轮没有新的 Windows 安装包。

### 安装前先核对

Windows 安装包 SHA-256：

```text
495a394bc9fd565cf18120a469c3eda145463f2c52d32a0901028e492320fefe
```

安卓 APK SHA-256：

```text
13314462f858e6dc88d834030d3ccce8c766be57d42ac43a1f73ede0078e789f
```

在 Windows 下载目录可运行：

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath '.\Offer-King-Setup-2.6.0.exe'
Get-FileHash -Algorithm SHA256 -LiteralPath '.\Offer-King-2.6.1-android-trial.apk'
```

核对大小与对应哈希；哈希一致只证明文件匹配，不代替数字签名、安全认证或安装兼容性。Windows 可能提示未知发布者／SmartScreen，安卓也可能有来源或调试包提示。只使用可信来源，遵循系统安全建议；不要关闭 Defender、SmartScreen、Play Protect 等保护。无法确认或持续被阻止时先停止，保留旧版并[反馈](https://github.com/YCC-Lover/Offer-King/issues/new?template=bug_report.yml)。

## 已有记录：先备份再升级

1. 在旧版“设置与备份”导出 JSON，确认文件存在并另存一份；附件原文件另行保管。
2. 关闭旧版，不清空数据目录，不为了更新先卸载。
3. Windows 保留原安装位置；设计上保留安装身份与数据，但真实覆盖安装未验收。升级后核对公司、岗位、附件和 AI 配置，再继续保管旧备份。
4. 安卓 2.6.0 及更早试用版需先手动下载 2.6.1 一次，打开 APK 并在原 App 上选择“更新”，不要卸载、清除数据或重置 AI。2.6.1 沿用 2.6.0 的应用 ID、页面存储来源、数据库与 AI 加密存储配置及 Debug 签名，设计为保留记录和 AI 配置；真机覆盖及升级后密钥解密未验收。提示签名不兼容时停止，保留旧 App。未来正式签名可能需要另行迁移。
5. JSON 不包含 AI 密钥和附件文件，请安全保管自己的密钥与附件。跨设备导入只迁移可支持的业务资料，不自动同步；桌面附件路径和手机文档授权不能直接互换，新设备需重新选择。

## 第一次使用与语言

安装成功后先用虚构资料验证“新增公司与岗位 → 保存 → 关闭重开 → 导出备份”，不用先配 AI。投递、比较、薪资试算等本地功能不要求应用账号或 AI 账号。

界面提供简体中文、English、日本語、한국어，语言可即时切换并保留已有输入，公司、岗位、备注与 AI 原文不会自动翻译。Windows 最小窗口 1100×700，字号 90%–125%；这个桌面窗口要求不适用于安卓手机，手机真实体验仍待反馈。

[Windows 图文上手](QUICKSTART.md) · [平台差异与 AI 设置](AI-SETUP.md) · [隐私](PRIVACY.md)

## 试用时先检查这五件事

先用虚构资料完成下面的检查，再决定是否录入重要记录。此清单是给试用者的建议，**不是维护者已完成真实安装验收的声明**。

- [ ] **能打开：** 使用对应平台的安装文件，打开后确认“帮助与关于”为 Android 2.6.1 或 Windows 2.6.0；遇到安全拦截先停止，不关闭防护。
- [ ] **能录入：** 新增一家公司和岗位，或粘贴虚构招聘文字，核对识别结果再保存；无需配置 AI。
- [ ] **能跟进：** 修改阶段、安排下一事项，打开详情并检查保存结果；手机也请检查滚动、返回键与软键盘是否遮挡。
- [ ] **重开还在：** 正常关闭、重新打开，检查公司、岗位与下一事项。未保存草稿和已保存记录不是同一件事。
- [ ] **能留备份：** 导出 JSON，确认导出文件存在并独立保管；不为测试清空现有数据，不公开上传自己的备份。

某一步不正常，先保留旧版与已有备份，用虚构资料记录步骤后[提交问题](https://github.com/YCC-Lover/Offer-King/issues/new?template=bug_report.yml)。安卓请补充系统版本和机型，不提供序列号或设备标识。

## 更新会自动发生吗？

Windows 2.6.0 在启动及使用期间可自动检查固定 GitHub 发布源，每天最多一次，也可手动检查、忽略或关闭。只在找到适配平台、严格更新版本和允许渠道的安装文件后提醒，打开官方发布页；**不自动下载或安装，不后台常驻**。

安卓 2.6.1 修复官方试用 APK 的识别：在“帮助与关于 → 应用更新”可手动检查，或开启前台自动检查和“同时接收候选试用版提醒”。自动检查最多每 24 小时一次，手动检查不受间隔限制；找到更高版本后打开对应发布页。已有关闭／忽略偏好会保留，检查版本不调用 AI。仅有当前版时显示“暂无更新”是正常的。

安卓 2.6.0 及更早试用版无法识别 trial 文件名，须先手动覆盖到 2.6.1；Windows 2.4.0 及更早公开版也须先手动升级。GitHub Watch 的通知来自 GitHub／邮箱；发布 Release 不会给旧 APK 远程添加功能。

## 分享与未验收事项

只分享所需平台的包、指南、校验清单和发布页，不分享项目、数据目录、备份或密钥。AI 使用自己的服务账户，免费额度与可用性由服务商决定；本地记录不因未配置 AI 而受限。

安卓 2.6.1 对应 1,291 项单元／组件、110 项原生 JVM 检查、27 项原生契约及六组移动浏览器仿真，APK 构建／验签／资产复验通过。Windows 2.6.0 沿用原测试记录。**安卓真机首装、覆盖、升级后 AI 解密和实际使用仍未验收；Windows 真实安装验收状态也未改变。** [安卓完整已测／未测](RELEASE-2.6.1.md#已验证与尚未验收) · [Windows 原范围](RELEASE-2.6.0.md#已验证与尚未验收)

<details>
<summary><strong>随包测试快照和发布后下载核验有什么区别？</strong></summary>

每个 Release 的 `TEST-RESULTS.json` 只记录该版本精确安装包对应的构建与测试范围；它不包含设备资料、密钥或本机证据路径。2.6.1 为安卓修复包，不能将它的测试结果套用到 Windows。文件通过 SHA-256 校验，不代表安装兼容性或真机体验已验收。

请将下载文件的完整 SHA-256 与本页及 `SHA256SUMS.txt` 对照。若下载不完整，重新从官方发布页下载，不运行残缺文件，不使用来源不明的替代包。旧版本的测试与下载核验记录不能当作本版本结果。

</details>

核对日期：2026-10-24。
