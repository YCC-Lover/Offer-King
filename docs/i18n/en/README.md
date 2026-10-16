<div align="center">

<img src="../../images/00-brand.png" width="88" height="88" alt="Offer King crown and application notes icon">

# Offer King

### Keep your applications on track. Make your next offer easier to choose.

A Windows desktop companion for managing applications, preparing for interviews, comparing offers, and planning life in a new city.

**Windows 10 / 11 · x64 · Four interface languages · Local data · No app account required · Optional AI**

[简体中文](../../../README.md) · **English** · [日本語](../ja/README.md) · [한국어](../ko/README.md)

**[Download 2.3.0 candidate](https://github.com/YCC-Lover/Offer-King/releases/download/v2.3.0/Offer-King-Setup-2.3.0.exe)** · [Download guide](DOWNLOAD.md) · [AI setup](AI-SETUP.md)

</div>

> [!IMPORTANT]
> **2.3.0 is a candidate release (Pre-release)** with Simplified Chinese, English, Japanese, and Korean. The installer is unsigned (**NotSigned**). Real clean installation, installation over an existing version, and uninstallation have **not yet completed acceptance testing**. Back up before trying an upgrade. [Release status, in Chinese](../../RELEASE-2.3.0.md#已验证与尚未验收)

![Offer King 2.3.0 English dashboard with synthetic applications](../../images/17-english-ui.png)

*English UI captured from the actual 2.3.0 packaged candidate using synthetic data, at 1400 × 900 and 100% text size, with external network access blocked. The Chinese company and job names deliberately demonstrate that user content stays unchanged. New users start with an empty database. [Screenshot notes](../../images/README.md)*

## Built around your job search

- **Track several companies at once.** Move applications through stages, keep an interview timeline, and give each role a next action and date. One company can have several independent applications.
- **Compare offers on your own terms.** Separate recurring annual compensation from first-year compensation. Use the two-offer comparison to weigh pay, growth, work–life balance, and your personal priorities.
- **Plan before moving.** Enter your own rent, commuting, living costs, and take-home cash to estimate savings. City budgets are personal estimates, not live market prices or automatic tax calculations.
- **Keep decisions grounded.** Review company information, risk research with sources, personal company rankings, and salary analysis together. Scores support your judgment; they are not objective company ratings.

![Application board, with a separate scrolling column for each stage](../../images/03-board.png)

*This older board screenshot is from 2.0.0 and uses synthetic data; it is not the 2.3.0 English interface.*

## Start in three steps

1. **Download and verify.** Follow the [download guide](DOWNLOAD.md). You do not need GitHub login or developer tools to download the public installer.
2. **Choose a language and save your first application.** Use the language selector in the sidebar or Settings & backup → Display & readability. Choose Add application, enter the company, role, city, and stage, then create the record. Add a next action when you know what comes next.
3. **Add details as they become useful.** Record compensation, compare offers, and export a JSON backup regularly. Keep original attachment files separately.

Language changes apply immediately and are remembered on this computer. Current edits remain in place; company names, job titles, notes, and custom stage names stay as written. Language settings are not part of job-data backups. AI can be configured later; local records, tasks, comparisons, and backups work without it. Older screenshots and the [detailed Chinese walkthrough](../../QUICKSTART.md) use Chinese labels.

## What is new in 2.3.0?

- **Four interface languages:** switch between 简体中文, English, 日本語, and 한국어 from the sidebar or display settings, without restarting.
- **Keep your words and edits:** changing interface language preserves current form input and stored company, application, note, and custom-stage text. Default stage labels are translated for display without rewriting stored stage names.
- **Guides in your language:** this homepage, the download guide, and the AI setup guide are available in all four languages.

The everyday features introduced in 2.2.0 remain available:

- **All reminders in one place:** overdue, today, the next seven days, later, and without a scheduled time. Completing an item creates a timeline event and clears that next action without changing its stage.
- **Recoverable drafts:** preview recovered two-offer and city-budget drafts after an unexpected exit, restore them, then explicitly save.
- **Extract pasted job descriptions:** review evidence-backed suggestions before adding them to a draft. This does not search the web or verify the source text.
- **AI configuration checks:** check the saved job model and search route after confirming quota and possible costs.

[Feature tour](../../FEATURES.md) · [Release notes](../../RELEASE-2.3.0.md) · [Changelog](../../../CHANGELOG.md)

## AI: choose when and how to use it

AI is optional. The app includes **no shared API key** and no promise of unlimited free cloud usage.

- To analyze a job description you already have, configure a compatible job model or a prepared local Ollama model. Search credentials are not required for this task.
- To research public information online, configure a model and the required search service. The free-start preset uses your own OpenRouter and Tavily accounts and keys; availability and quotas depend on those providers.
- Existing Bailian and DeepSeek configurations remain available. Model connections, searches, and tests may consume quota or incur charges.

Automatic research after creating a new application is off by default. AI suggestions need your review and an explicit save. [English AI setup guide](AI-SETUP.md)

## Common questions

<details>
<summary><strong>Can I use it offline and without AI?</strong></summary>

Yes. Local records, application stages, timelines, reminders, comparisons, budgets, and backups do not require AI. Reminders are shown inside the app; they are not alarms that run after you close it. Website icons and AI features may access the network.

</details>

<details>
<summary><strong>Will friends receive my applications or keys?</strong></summary>

No. The installer does not include the author's data or keys. Everyone starts with their own local records and configures their own services. Share the installer or project link, not your personal data folder or backups.

API keys are encrypted on the local computer and excluded from job-data JSON backups. Records, recovery drafts, and backups are not an encrypted vault. Attachments are stored as file paths; backup files do not contain the attachment files themselves.

Cloud text extraction sends the text you paste to your selected model. The complete pasted text is kept only in the current window's memory; accepted fields and limited evidence excerpts can remain in drafts, records, and backups. Remove private information before submitting. [Privacy details, in Chinese](../../PRIVACY.md)

</details>

<details>
<summary><strong>What languages and platforms are available?</strong></summary>

The 2.3.0 candidate supports Simplified Chinese, English, Japanese, and Korean on Windows 10 / 11 x64. Switch from the sidebar or display settings; the preference is stored locally and takes effect immediately. Existing 2.2.0 downloads retain their Chinese interface. There are currently no macOS, Linux, mobile, portable, cloud-sync, or collaboration editions, and no automatic updater.

</details>

## Feedback and sharing

[Report a bug](https://github.com/YCC-Lover/Offer-King/issues/new?template=bug_report.yml) · [Suggest a feature](https://github.com/YCC-Lover/Offer-King/issues/new?template=feature_request.yml) · [Correct a translation](https://github.com/YCC-Lover/Offer-King/issues/new?template=docs_feedback.yml)

English, Japanese, Korean, and Chinese feedback is welcome. Include your version, Windows version, steps, expected result, and actual result. For layout issues, add language, font size, theme, and Windows display scaling. Public Issues must not contain keys, complete backups, private attachments, or unredacted personal paths. [Feedback guide](../../../CONTRIBUTING.md) · [Private security reporting](../../../SECURITY.md)

If Offer King helps, you can Star the [project](https://github.com/YCC-Lover/Offer-King), share it with a friend, or use GitHub Watch → Releases for release notifications.

---

[中文文档中心](../../README.md) · [All releases](https://github.com/YCC-Lover/Offer-King/releases) · [License](../../../LICENSE.md) · [Third-party notices](../../../THIRD-PARTY-NOTICES.txt)

Offer King is closed-source software. This public repository contains download links, documentation, and feedback channels, not the application source code. Documentation updated 2026-10-16.
