<div align="center">

<img src="../../images/00-brand.png" width="88" height="88" alt="Offer King crown and application notes icon">

# Offer King

### Keep your applications on track. Make your next offer easier to choose.

A local-first job-search companion: follow up on applications, compare offers, and plan your next move.

**Windows 10 / 11 x64 + Android trial · Four UI languages · Local records · No app account required · AI optional**

[简体中文](../../../README.md) · **English** · [日本語](../ja/README.md) · [한국어](../ko/README.md)

**[Download Windows 2.6.0](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.0/Offer-King-Setup-2.6.0.exe)** · **[Download Android 2.6.1](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.1/Offer-King-2.6.1-android-trial.apk)**

[Download & verification guide](DOWNLOAD.md) · [AI setup](AI-SETUP.md) · [Android 2.6.1 release notes](../../RELEASE-2.6.1.md)

</div>

> [!IMPORTANT]
> **Android 2.6.1 and Windows 2.6.0 are trial candidates (Pre-release), not production releases.** This update is Android-only; Windows stays at 2.6.0. Windows is **NotSigned**; Android has a **Debug development/test signature**, not a production identity.
> Windows clean/upgrade installation and uninstallation, and Android real-device installation, upgrade and runtime use, **have not completed acceptance testing**. Export a backup before upgrading; if Android reports a signature conflict, stop rather than uninstalling your existing app.
> No macOS, iOS or Linux installer is available.

## Built around your job search

For people managing several applications, weighing offers, or considering a move:

- **Follow every application.** Use stage boards, interview timelines, next actions and dates. Several roles at one company can progress independently.

- **Type less.** Paste one job posting, review evidence recognized on-device, and fill selected empty fields. Existing input and a reused company's shared details stay intact; ambiguous information is not guessed.

- **Compare what matters.** Separate recurring annual compensation from first-year compensation; compare two offers using your own priorities.

- **Estimate take-home pay.** Explore mainland-China CNY social-insurance, housing-fund and tax estimates across 12 months. Calculations never rewrite the original job's compensation.

- **Plan a move.** Enter your rent, commuting and living costs to estimate savings. City budgets use your assumptions, not live market prices.

- **Keep decisions grounded.** Bring company information, sourced risk research and personal top-three rankings together. Scores are decision aids, not objective company ratings.

[Explore the features](../../FEATURES.md)

## Start in three steps

1. **Download and verify.** Pick the Windows installer or Android trial above, then follow the [download guide](DOWNLOAD.md). No GitHub login or developer tools are needed to download the public files.

2. **Create your first application.** Choose a UI language, enter the company and role, or paste a posting for an offline preview. Confirm the city and stage; reuse an existing company when appropriate. Add a next action and date when known.

3. **Save, then back up.** Add details when useful, explicitly save your changes, and export JSON regularly. Keep original attachment files separately. You can configure AI later.

Language switches take effect immediately and stay on this device. **Your company names, job titles, notes and custom stage names are not translated.** Current edits remain in place; the language preference is not part of job-data backups.

[Detailed walkthrough, in Chinese](../../QUICKSTART.md)

## See the interface

![Actual Offer King 2.3.0 English dashboard with synthetic applications](../../images/17-english-ui.png)

*Actual English UI from the 2.3.0 packaged candidate, using synthetic data at 1400 × 900 and 100% text size, with external network access blocked. This is not a 2.6.0 or Android screenshot. Chinese company/job names demonstrate unchanged user content; new users start empty. [Screenshot sources](../../images/README.md)*

<details>
<summary>Older application-board example — 2.0.0</summary>

![Offer King 2.0.0 application board with synthetic records](../../images/03-board.png)

This older Chinese-interface screenshot shows the board layout with synthetic data, not the current English UI or Android app.

</details>

## New in the Android 2.6.1 trial

- **Check for future trial updates inside the app.** Help & about → App updates supports manual checks and automatic foreground checks at most once per 24 hours when enabled. Include candidate releases must be on, and ignored-version preferences still apply. A notice opens the official release page; you choose whether to download and install.
- **Upgrade once manually from 2.6.0 or earlier.** Those Android trial builds do not recognize trial APK filenames. Install 2.6.1 over the existing app to gain the corrected checker; no remote change can add it to an old APK.
- **Keep the existing installation.** The app ID, data origin, AI storage and 2.6.0 Debug signer are retained by design. Export JSON outside the app first, keep attachments separately, and do not uninstall, clear data or reset AI settings. JSON excludes keys and attachment files. Real-phone first installation, in-place upgrade and encrypted-key retention remain unaccepted; stop if the signature conflicts.
- **Read update notices in dark mode.** The update card has clearer text contrast. Checking releases does not use AI, send your records or keys, or incur AI charges; AI configuration and routes are unchanged.

[Android 2.6.1 release](https://github.com/YCC-Lover/Offer-King/releases/tag/v2.6.1) · [Upgrade instructions](DOWNLOAD.md#trying-or-upgrading-android)

## Retained from the 2.6.0 trial

- **Find the next record faster.** Open local quick find from the header or with `Ctrl/Cmd + K`; search pages, companies and jobs, then navigate with the keyboard.
- **Work in a board or a list.** Switch views, combine six filters (stage, priority, city, work mode, favorites and reminders), sort, and save up to **12 named views**. Lists show **30 records per page**; views store presentation preferences, not copies of your records or search text.
- **Follow up without opening a long form.** Edit the next action and date from a board/list card or reminder, then explicitly save. Successful changes enter the timeline without moving the job's stage.
- **Focus on today's work.** A more compact home prioritizes reminders; details reveal secondary fields on demand. Mobile layouts preserve readable large text, scrolling and fixed actions.

These additions work locally and do not call AI. Automatic research remains off by default. Verification passed **1,280 unit/component tests**, **314 Node tests** (4 skipped), **5 packaged Electron scenarios**, and **one unpacked 2.5.4 → 2.6.0 upgrade scenario using synthetic data**. Android compiled and passed static package checks; browser touch/layout checks are not phone acceptance. Actual Windows installation and Android real-device acceptance are still pending.

[Read the full 2.6.0 notes](../../RELEASE-2.6.0.md) · [Release page](https://github.com/YCC-Lover/Offer-King/releases/tag/v2.6.0) · [Version history](../../../CHANGELOG.md)

## AI: choose when and how to use it

**Start without AI.** Pick the path that matches what you need:

1. **Offline, no setup:** local records, quick entry and take-home estimates need no model, key, network connection or AI fee.

2. **Model-only extraction:** analyze a job description you already have using a compatible configured model. A prepared local Ollama setup is another option where supported. This does not search the web or verify the original text; no search key is required.

3. **Model + search:** research public company/job information using a supported model and the required search route. The OpenRouter + Tavily starter preset still needs **your own accounts and keys**.

There is **no bundled shared API key or guaranteed free cloud quota**. Model calls, searches and connection tests may consume quota or incur charges; provider availability and compatibility vary. Existing Bailian/DeepSeek options and platform limits are explained in the [AI setup guide](AI-SETUP.md).

Automatic research after creating an application is **off by default**. Check sources and dates, select suggestions into the draft, then **explicitly save**. AI output is not verified fact and does not silently overwrite records.

## Common questions

<details>
<summary><strong>Can I use it offline and without an account?</strong></summary>

Yes: local records, stages, timelines, next actions, comparisons, budgets and JSON backups need neither an app account nor AI. There is no cloud sync or collaboration. Reminders appear inside the app, not as alarms after it closes; website icons and AI features may use the network.

</details>

<details>
<summary><strong>Is the salary calculator international?</strong></summary>

No. It estimates CNY pay for mainland Chinese resident employees, assuming a fixed monthly salary for 12 months with the same employer from January. Choose your actual contribution bases/rates for any city; the Beijing reference template applies only when explicitly selected. This is not international payroll or tax advice, and foreign-currency pay is not silently converted. Results do not write back to jobs or city budgets.

</details>

<details>
<summary><strong>What should I back up or share with friends?</strong></summary>

Share the installer or project link, not your personal data folder or backups. Installers contain no author's records or keys; each person starts with their own local data. Keys use platform secure storage and are excluded from job-data JSON, but records, recovery drafts and backups are **not an encrypted vault**.

JSON backups do **not** contain attachment files. Windows attachments retain local paths; Android attachments use device-specific document authorization, which does not transfer with the backup. Keep the originals separately.

Cloud extraction sends pasted text to your selected model. The full paste is memory-only, but accepted fields and limited evidence excerpts can remain in drafts, records and backups. Remove private information before submitting. [Privacy details, in Chinese](../../PRIVACY.md)

</details>

<details>
<summary><strong>How do I update? Which platforms and languages are available?</strong></summary>

Windows 2.5.4 and later can check releases while open and foregrounded, manually or once per 24 hours automatically when enabled; enable **Include candidate releases** for Windows 2.6.0. Windows 2.4.0 and earlier need a manual upgrade first. **Android trial 2.6.0 and earlier also need one manual upgrade to 2.6.1** to recognize future official trial APKs. From 2.6.1, use Help & about → App updates and enable candidate releases; disabled automatic checks and ignored versions are respected. Notices open the official release page and **never download or install automatically**. Stop on a signature conflict rather than deleting existing data. [Backup and upgrade guide](DOWNLOAD.md)

The published trial covers Windows 10 / 11 x64 and Android 7.0+ with Simplified Chinese, English, Japanese and Korean UI. Real-device acceptance remains pending. No macOS/iOS/Linux installer or portable edition is available. The 1100 × 700 minimum window is Windows-only, not an Android requirement.

</details>

## Feedback and sharing

[Report a bug](https://github.com/YCC-Lover/Offer-King/issues/new?template=bug_report.yml) · [Suggest a feature](https://github.com/YCC-Lover/Offer-King/issues/new?template=feature_request.yml) · [Correct a translation](https://github.com/YCC-Lover/Offer-King/issues/new?template=docs_feedback.yml)

Feedback in all four languages is welcome. Include the app/OS versions, reproduction steps, expected and actual results. For layout issues, add language, text size, theme and desktop scaling or phone orientation. Public Issues must not contain keys, complete backups, private attachments or unredacted personal paths.

[Feedback guide](../../../CONTRIBUTING.md) · [Private security reporting](../../../SECURITY.md)

If it helps your search, Star the [project](https://github.com/YCC-Lover/Offer-King) or share it with a friend. GitHub Watch → Releases is separate from the app's update checks.

---

[Chinese documentation hub](../../README.md) · [All releases](https://github.com/YCC-Lover/Offer-King/releases) · [License](../../../LICENSE.md) · [Third-party notices](../../../THIRD-PARTY-NOTICES.txt)

Offer King is closed-source software. This public repository provides downloads, documentation and feedback channels, not the application source code. Documentation updated **2026-10-24**.
