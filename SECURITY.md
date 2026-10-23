# 安全反馈

**中文或 English 都可以。** Please report potential vulnerabilities privately. Do not include real keys, personal records, private attachments or device identifiers.

如果发现可能泄露数据、执行非预期代码或绕过安全限制的问题，请使用本仓库 **Security → Report a vulnerability** 发起私密报告：

[提交私密安全报告](https://github.com/YCC-Lover/Offer-King/security/advisories/new)

只提供复现所必需的合成示例、受影响版本和环境。不要发送真实 API Key、求职备份、联系人或私人附件。请勿在公开 Issue 中发布敏感细节、可用凭据或针对他人的数据。

若私密入口暂不可用，请使用[文档反馈表](https://github.com/YCC-Lover/Offer-King/issues/new?template=docs_feedback.yml)，把标题改为“需要私密安全联络 / Private security contact needed”。“哪一页”只填 `SECURITY.md`，“问题”只填“私密报告入口不可用，需要私密联络渠道”。不要填写漏洞细节、复现代码、凭据或个人资料，也不要附文件；等待维护者提供合适的私密渠道。本仓库关闭了空白 Issue，此入口仅用于请求联络，不是公开报告漏洞的替代方式。

## 使用者可以做的事

- 仅从本仓库 Releases 下载对应平台文件，核对 SHA-256；不要关闭 Defender、SmartScreen、Play Protect 等系统防护。
- 2.6.0 Windows 包未正式签名；Android APK 使用开发测试签名，不是未签名，也不是正式发布证书。哈希一致只证明文件匹配，不代表 Microsoft、Google 或 GitHub 的安全认证。
- 真实 Windows 首装、覆盖安装、卸载及 Android 真机运行尚未验收；自动化测试或 APK 编译通过不能替代这些验证。没有 macOS／iOS 安装包。
- 升级前导出并妥善保管备份，附件原文件另存；API Key 不在 JSON 备份中。Android 签名不同可能无法覆盖，不要为绕过冲突直接卸载旧 App，也不要通过清空数据目录解决问题。
- 版本检查只读取固定官方 GitHub 发布信息；Windows 有可关闭的前台提醒，不自动下载或安装。Android Debug 试用文件不作为正式升级匹配资产；应用不会替你确认某个签名是否兼容旧安装。
- AI Key 仅在自己的 App 中配置，不向他人发送；如不慎泄露，及时到服务商控制台撤销并更换。

本项目由个人维护，不提供全天候安全响应或服务等级保证。当前重点维护 2.x 分支；旧版本未必收到单独补丁。
