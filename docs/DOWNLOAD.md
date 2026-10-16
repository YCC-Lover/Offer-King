# 下载 Offer King

[简体中文](DOWNLOAD.md) · [English](i18n/en/DOWNLOAD.md) · [日本語](i18n/ja/DOWNLOAD.md) · [한국어](i18n/ko/DOWNLOAD.md)

[项目首页](../README.md) · [文档中心](README.md) · [功能导览](FEATURES.md) · [AI 配置](AI-SETUP.md)

**Windows 上的本地求职与 Offer 决策助手。** 安装后就能记录投递、安排面试、比较待遇；不需要开发工具、应用账号或 AI 账号。

## Windows 下载

### [下载 2.3.0 候选试用版 · Windows x64](https://github.com/YCC-Lover/Offer-King/releases/download/v2.3.0/Offer-King-Setup-2.3.0.exe)

大小：**111,824,372 字节／106.6 MiB** · [发布页与更新说明](https://github.com/YCC-Lover/Offer-King/releases/tag/v2.3.0) · [安装后开始使用](QUICKSTART.md#2-建立第一条投递)

> **2.3.0 为支持四语切换的候选试用版（Pre-release）。** 安装包未签名（NotSigned），真实干净 Windows 首装、覆盖安装和卸载尚未验收。旧用户请先导出备份。[查看已测与待测范围](RELEASE-2.3.0.md#已验证与尚未验收)

公开下载无需 GitHub 登录。以下三个文件都来自同一个固定版本发布页：

- **[Offer-King-Setup-2.3.0.exe](https://github.com/YCC-Lover/Offer-King/releases/download/v2.3.0/Offer-King-Setup-2.3.0.exe)**：安装 App，下载后按安装向导操作。
- **[SHA256.txt](https://github.com/YCC-Lover/Offer-King/releases/download/v2.3.0/SHA256.txt)**：核对这份安装包的文件校验值。
- **[START-HERE.txt](https://github.com/YCC-Lover/Offer-King/releases/download/v2.3.0/START-HERE.txt)**：便于下载后离线查看的入门说明与反馈入口。

GitHub 自动生成的 `Source code` 压缩包是本公开仓库的文档，不是安装包，也不包含应用源码。不要使用“Code → Download ZIP”来安装 App。

## 这台电脑可以用吗？

| 项目 | 当前版本 |
| --- | --- |
| 系统 | Windows 10 / 11，x64 |
| 语言 | 简体中文、English、日本語、한국어；侧栏或显示设置中即时切换 |
| 窗口 | 最小 1100 × 700；字号可在设置中调整为 90%–125% |
| 安装 | Windows 安装程序；未提供便携版 |
| 离线 | 无需应用账号，记录、比较与备份可离线使用 |
| AI | 可选；使用自己的模型和密钥，调用可能产生费用 |
| 平台 | 尚无 macOS、Linux 或手机安装版 |

**首次使用：** 安装后从自己的空白资料开始，先[建立第一条投递](QUICKSTART.md#2-建立第一条投递)。AI 可以以后再配；安装包不含作者的记录或共享密钥。

语言可随时切换，并在本机记住选择。正在编辑的输入不清空，公司、岗位、备注和人工阶段名保留原文；切换语言不代表翻译已有 AI 调研内容，也不更改模型或密钥配置。

<details>
<summary><strong>安装前核对文件与 Windows 提示</strong></summary>

在安装包所在文件夹打开 PowerShell，运行：

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath '.\Offer-King-Setup-2.3.0.exe'
```

2.3.0 文件大小应为 **111,824,372 字节**，SHA-256 应为：

```text
E3F0793EE439D6975C45CA566BBE07D077C62416F5753329C73435C2DC037463
```

哈希核对文件是否一致，不是数字签名或安全认证。不同版本需要核对各自发布页的值。

未签名的安装包可能出现“未知发布者”或 SmartScreen 提示。请确认下载来源，遵循系统安全建议；不要关闭 Defender、SmartScreen 等防护。无法确认或持续被拦截时先停止安装，再[反馈问题](https://github.com/YCC-Lover/Offer-King/issues/new?template=bug_report.yml)。

</details>

<details>
<summary><strong>已经使用旧版：备份与升级顺序</strong></summary>

1. 在旧版“设置与备份”中手动导出 JSON，保存到自己能妥善保管的位置；附件原文件另外保管。
2. 关闭旧版，保留原安装位置。不要为了更新先清空应用数据或卸载。
3. 确认接受候选试用范围后运行安装程序。启动新版，核对公司、岗位和 AI 配置状态，并继续保留升级前备份。
4. 出现异常时保留现状并反馈，不要清空数据或用旧备份直接覆盖尚未检查的资料。

版本设计保留原安装身份与数据位置；2.3.0 最终兼容性验证结果以本版发布说明为准，合成资料测试也不能代替真实安装器覆盖验收。JSON 不包含 API Key、未提交草稿或附件文件本身。换电脑需要另外迁移附件、重新配置自己的 AI 密钥。[完整备份说明](QUICKSTART.md#8-做好备份再慢慢完善)

当前没有自动更新。GitHub 的 Latest 标记可能指向其他版本，也不代表本页的 2.3.0 已完成安装验收；请使用本页固定链接获取本候选版。

</details>

## 分享与下一步

把本页链接或安装包与指南分享给朋友即可。每个人的求职资料保存在各自电脑上，各自配置 AI 密钥；不要分享自己的数据目录、备份或密钥。

[图文上手](QUICKSTART.md) · [AI 配置与排错](AI-SETUP.md) · [数据与隐私](PRIVACY.md) · [常见问题](FAQ.md) · [反馈问题](../CONTRIBUTING.md)

下载信息核对：2026-10-16。安装包身份与验证范围以 [2.3.0 发布说明](RELEASE-2.3.0.md)为准。
