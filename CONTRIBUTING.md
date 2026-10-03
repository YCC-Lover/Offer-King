# 一起把下一版用得更顺手

你不需要会写代码。一个清楚的使用场景，比一句“建议优化一下”更容易变成下一版的改进。

## 选择合适的入口

- **操作不正常**：[报告 Bug](https://github.com/YCC-Lover/Offer-King/issues/new?template=bug_report.yml)。请给出版本、系统、步骤，以及期望和实际结果。
- **想要新能力**：[提出功能建议](https://github.com/YCC-Lover/Offer-King/issues/new?template=feature_request.yml)。先说你遇到的麻烦，再说设想中的操作方式。
- **教程看不懂**：[改进文档](https://github.com/YCC-Lover/Offer-King/issues/new?template=docs_feedback.yml)。告诉我们卡在哪一页、哪一步。
- **潜在安全问题**：请先看 [安全说明](SECURITY.md)，不要在公开 Issue 中贴密钥或漏洞细节。

提交前搜索已有 Issue；遇到相同问题，可以补充信息或使用 👍，不必重复建单。公开反馈需要 GitHub 账号，下载和使用 App 不需要。

## 保护你自己，也保护他人

Issue 和截图对所有人可见。请遮住姓名、电话、邮箱、公司内部信息、薪酬、真实文件路径与 API Key。不要上传求职 JSON 备份、数据库、完整日志或整个用户数据目录。App 的“帮助与关于”有反馈模板和脱敏诊断入口；发送前仍请自行检查。

## 反馈之后会发生什么？

维护者会先复现或补充了解，再决定处理范围。常见标签：

| 标签 | 含义 |
|---|---|
| `needs-triage` | 已收到，等待核对 |
| `bug` / `enhancement` / `documentation` | 问题类型 |
| `planned` | 已明确纳入后续安排 |
| `in-progress` | 正在实现或验证 |
| `released` | 已随版本交付，请查看更新说明 |

优先关注数据安全、无法使用的流程与可读性问题；不保证每条建议都实现，也不承诺固定响应时限。查看 [路线图](ROADMAP.md) 和 [更新记录](CHANGELOG.md) 了解进展。

本仓库不接受应用源码 PR，因为应用源码不公开；欢迎针对公开教程、错别字和可访问性说明提出文档 PR。请不要提交第三方机密材料或未经授权的图片。
