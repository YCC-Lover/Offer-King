# 下载 Offer King 2.5.4

[简体中文](DOWNLOAD.md) · [English](i18n/en/DOWNLOAD.md) · [日本語](i18n/ja/DOWNLOAD.md) · [한국어](i18n/ko/DOWNLOAD.md)

[项目首页](../README.md) · [文档中心](README.md) · [功能导览](FEATURES.md) · [AI 配置](AI-SETUP.md)

**候选试用版（Pre-release），无需应用账号；AI 可选。** 不设试用到期时间，不人为限制本地功能。每个人从自己的本机空数据开始，设备之间不自动同步。

> Windows 未正式数字签名；安卓带开发测试签名。真实 Windows 首装、覆盖安装和卸载，以及安卓真机安装、覆盖与使用均未验收。愿意接受这些限制再试用，升级前先导出 JSON。不要关闭系统安全防护或因签名冲突直接卸载旧应用。

## 选择你的平台

| 平台 | 固定 2.5.4 下载 | 大小／说明 |
| --- | --- | --- |
| Windows 10/11 x64 | [Offer-King-Setup-2.5.4.exe](https://github.com/YCC-Lover/Offer-King/releases/download/v2.5.4/Offer-King-Setup-2.5.4.exe) | 112,083,805 字节；NotSigned；NSIS 安装包 |
| Android | [Offer-King-2.5.4-android-trial.apk](https://github.com/YCC-Lover/Offer-King/releases/download/v2.5.4/Offer-King-2.5.4-android-trial.apk) | 33,702,975 字节；Debug 签名；真机未验收 |
| macOS / iOS / Linux | 暂无安装包 | 源码准备或另一平台编译成功，不等于已有可安装版本 |

[固定发布页](https://github.com/YCC-Lover/Offer-King/releases/tag/v2.5.4) · [更新与实际验收范围](RELEASE-2.5.4.md)

GitHub 的 Latest 可能仍指向旧正式标记；请使用本页固定链接。公开下载不要求 GitHub 登录，也不需要开发工具。`Source code` ZIP 仅是本公开仓库的文档，不是安装包或应用源码。

## 一起下载的说明与校验

- [SHA256SUMS.txt](https://github.com/YCC-Lover/Offer-King/releases/download/v2.5.4/SHA256SUMS.txt)：两个包、离线指南和测试摘要的校验值。
- [START-HERE.md](https://github.com/YCC-Lover/Offer-King/releases/download/v2.5.4/START-HERE.md)：可离线阅读、随安装包分享的上手与 AI 说明。
- [TEST-RESULTS.json](https://github.com/YCC-Lover/Offer-King/releases/download/v2.5.4/TEST-RESULTS.json)：实际通过、跳过和未验收范围，不含个人资料。

### 安装前先核对

Windows 安装包 SHA-256：

```text
75b19b121a9736c2b46c62cca9e40333b4f4e8e92528b34d4a10bbe4e4de7a8d
```

安卓 APK SHA-256：

```text
85ca9c2f67be4ede787016e6b9487d50f359c7171b271afe8dfe022feceab89c
```

在 Windows 下载目录可运行：

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath '.\Offer-King-Setup-2.5.4.exe'
Get-FileHash -Algorithm SHA256 -LiteralPath '.\Offer-King-2.5.4-android-trial.apk'
```

核对大小与对应哈希；哈希一致只证明文件匹配，不代替数字签名、安全认证或安装兼容性。Windows 可能提示未知发布者／SmartScreen，安卓也可能有来源或调试包提示。只使用可信来源，遵循系统安全建议；不要关闭 Defender、SmartScreen、Play Protect 等保护。无法确认或持续被阻止时先停止，保留旧版并[反馈](https://github.com/YCC-Lover/Offer-King/issues/new?template=bug_report.yml)。

## 已有记录：先备份再升级

1. 在旧版“设置与备份”导出 JSON，确认文件存在并另存一份；附件原文件另行保管。
2. 关闭旧版，不清空数据目录，不为了更新先卸载。
3. Windows 保留原安装位置；设计上保留安装身份与数据，但真实覆盖安装未验收。升级后核对公司、岗位、附件和 AI 配置，再继续保管旧备份。
4. 安卓签名不同不能直接覆盖。当前包沿用此前开发包的 Debug 身份，但没有手机覆盖实测；将来正式签名可能需要迁移。出现冲突先保留旧 App，不直接卸载。
5. 跨设备导入 JSON 只迁移可支持的业务资料，不自动同步；AI 密钥不在备份中，桌面附件路径和手机文档授权不能直接互换，需在新设备重新选择。

## 第一次使用与语言

安装成功后先用虚构资料验证“新增公司与岗位 → 保存 → 关闭重开 → 导出备份”，不用先配 AI。投递、比较、薪资试算等本地功能不要求应用账号或 AI 账号。

界面提供简体中文、English、日本語、한국어，语言可即时切换并保留已有输入，公司、岗位、备注与 AI 原文不会自动翻译。Windows 最小窗口 1100×700，字号 90%–125%；这个桌面窗口要求不适用于安卓手机，手机真实体验仍待反馈。

[Windows 图文上手](QUICKSTART.md) · [平台差异与 AI 设置](AI-SETUP.md) · [隐私](PRIVACY.md)

## 更新会自动发生吗？

Windows 2.5.4 在启动及使用期间可自动检查固定 GitHub 发布源，每天最多一次，也可手动检查、忽略或关闭。只在找到适配平台、严格更新版本和允许渠道的安装文件后提醒，打开官方发布页；**不自动下载或安装，不后台常驻**。

2.4.0 及更早公开版本没有该能力，需先手动升级一次。安卓 Debug 包不作为正式自动升级资产推荐。GitHub Watch 的通知来自 GitHub／邮箱，不会替你安装；不要把发布 Release 等同于给所有旧 App 推送。

## 分享与未验收事项

只分享所需平台的包、指南、校验清单和发布页，不分享项目、数据目录、备份或密钥。AI 使用自己的服务账户，免费额度与可用性由服务商决定；本地记录不因未配置 AI 而受限。

已完成 1214 项单元／组件检查、Windows 打包程序冒烟与界面检查、安卓构建和静态验包；这些不替代真实首装、覆盖、卸载、安卓设备运行或真实付费 AI 验收。[完整已测／未测](RELEASE-2.5.4.md#已验证与尚未验收)

核对日期：2026-10-19。
