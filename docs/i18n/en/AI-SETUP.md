# Offer King 2.5.4 AI setup

[简体中文](../../AI-SETUP.md) · [English](AI-SETUP.md) · [日本語](../ja/AI-SETUP.md) · [한국어](../ko/AI-SETUP.md)

[English home](README.md) · [Download](DOWNLOAD.md) · [Detailed Chinese guide](../../AI-SETUP.md)

This guide describes the **2.5.4 small-group trial, a Pre-release, not Latest**. There is no trial expiry or extra feature lock. Switch between Simplified Chinese, English, Japanese, and Korean in the sidebar or display settings; switching preserves current input and takes effect immediately. [Download and verification](DOWNLOAD.md) · [2.5.4 release, checksums and trial instructions](https://github.com/YCC-Lover/Offer-King/releases/tag/v2.5.4)

The steps below include Chinese labels in addition to English descriptions so they can also be followed with older screenshots. Interface language changes do not translate your records or change your AI provider, key, model, search route, or billing consent.

You can manage applications, tasks, offers, and backups without AI. AI is optional, uses your own accounts and keys, and may consume quota or incur charges. **No shared key or unlimited free service is included.**

### Check your platform first

| Platform | Trial file and verification limits | AI-specific differences |
| --- | --- | --- |
| Windows 10/11 x64 | `Offer-King-Setup-2.5.4.exe`, without a formal code signature. Packaged-app checks do not establish clean-install, upgrade-install or uninstall acceptance; those remain untested | Compatible cloud models, OpenRouter＋Tavily, the original Bailian/DeepSeek routes and local Ollama are implemented; keys use Electron secure storage |
| Android | `Offer-King-2.5.4-android-trial.apk`, signed with a development/test certificate. Compiled and mock-tested, not accepted on a real phone | Native model tests/listing, text extraction and company/job/risk research are implemented; keys use Android Keystore. Ollama loopback addresses mean the phone, not your PC |
| macOS / iPhone / iPad | No installable package is provided in this release | Source and simulated tests are not a tested Apple build |

New users on a fresh installation start with empty data until they import a backup; upgrades do not deliberately clear existing records. There is no cloud sync or bundled author account, records or keys. Back up before upgrading. If Android reports a signature mismatch, do not simply uninstall the old app: export and verify a backup before deciding how to migrate. JSON backups do not contain API keys or attachment files. The release assets `START-HERE.md`, `SHA256SUMS.txt` and `TEST-RESULTS.json` document setup, file checks and tested/untested scope.

## Start without AI

In **Add application → Paste a job posting**, use offline recognition to preview explicit company, role, city, links and salary fields, then choose which empty inputs to fill. Existing input and shared details of a reused company stay unchanged. Ambiguities are not guessed; amounts with no clear currency start unchecked. Complete text stays only in the window's memory and is not saved in recovery drafts or backups. This is not the AI text-extraction feature below: it needs no key or network access and incurs no AI fees.

The **Take-home pay** page also runs locally without a model or AI fees. It estimates CNY pay for mainland Chinese residents over 12 fixed-salary months with the same employer from January. Choose any city and enter actual contribution bases/rates; only Beijing currently has a verified reference template, applied only on explicit request. Results do not write back to job compensation or city budgets, do not convert foreign currencies, and are estimates rather than payroll or tax advice.

## 1. Choose the task first

| What you want | Configuration needed | Web search? |
| --- | --- | --- |
| Recognize explicit fields before creating a job, or estimate take-home pay | None; local tools | No AI or network calls |
| Use AI to extract more fields from a job description you paste | Compatible job model, or a prepared local Ollama model | No; Tavily is not required |
| Research public company or job information | Compatible model plus your Tavily key, or the existing provider route | Yes; review the sources |
| Keep local records, tasks, comparisons, and backups | None | No AI calls |

Text extraction **does not verify the description online**. An ordinary model does not gain web search just because you supply its API key. A successful model connection does not establish that search or structured extraction will work. Website logos and update checks are separate network features; using local recognition does not mean the whole app never connects to the internet.

## 2. Free-start preset

1. Open **设置与备份 → AI 调研 → 免费 AI 起步** (Settings & backup → AI research → Free AI start).
2. Create your own key at [OpenRouter](https://openrouter.ai/settings/keys) and enter it in “OpenRouter 免费模型 API Key”. The preset uses `openrouter/free` at `https://openrouter.ai/api/v1`.
3. Obtain your own search key from [Tavily](https://app.tavily.com/home) and enter “免费起步 Tavily API Key”. Check both services' current quotas and billing settings if you intend to stay within free allowances.
4. Click **保存并启用免费配置** (Save and enable free configuration). This explicitly switches company, job, and risk tasks to the preset; saving alone does not start research.
5. Run the model and search tests, or use the one-click check after reading the cost notice. Tests may use quota.

The free preset also requests zero-priced providers; it does not silently replace a failed free model with a paid one. Free-model availability and provider allowances can change, and the app promises neither a fixed quota nor permanent free use. Tavily is a search service, not a chat model, and has separate quotas and billing. On this route, each new research round uses at most one basic Tavily search without automatically increasing search depth; choosing a still-valid match reuses the first search evidence. Provider-side billing settings remain your responsibility. See the official [OpenRouter free-router guide](https://openrouter.ai/docs/guides/routing/routers/free-router) and [Tavily credit explanation](https://docs.tavily.com/documentation/api-credits).

“创建岗位后自动调研” (Research automatically after creating a job) is **off by default**. To opt in, enable it and click “保存自动调研偏好”. It runs once after a new application is successfully created, not while typing and not automatically for old applications.

## 3. Use your own model

Open **我的模型配置 → 新增模型配置** (My model configurations → Add configuration). Enter a recognizable name, protocol, base URL, exact model ID, and the corresponding API key. Supported routes include OpenAI-compatible Chat Completions, Responses, and local Ollama; the service/model must support the structured output the app requires. A chat website subscription does not necessarily include API access.

Cloud endpoints must be public HTTPS addresses. Check the normalized base address before saving. Read model IDs with “读取模型列表” or enter an exact ID manually if listing is unavailable.

**Saving a model does not enable it.** Test the saved model, then choose “设为默认并保存” or save the desired default/task assignments. Separate task overrides continue to apply; check the model card's actual scope. When changing service endpoints or protocols, provide the key for the new service.

For online research with compatible models, save and test your key in **联网搜索 · Tavily**. Text-only extraction does not need it. Advanced settings can assign separate models to company, job, and risk tasks. A failed selected route is reported rather than silently switching to another paid service.

### Local Ollama

On Windows, install and run Ollama yourself and download a suitable local model. Choose “Ollama 本机模型”; the default endpoint is `http://127.0.0.1:11434/v1`, and no API key is needed. The app connects only to the local loopback service and does not install Ollama or download models for you. See [Ollama's compatibility documentation](https://docs.ollama.com/api/openai-compatibility).

**On Android, `localhost`, `127.0.0.1` and `::1` mean the phone itself, not your PC.** The local route does not accept your computer's LAN address, and the APK does not include a phone model server. Unless you have prepared a compatible service on the phone, use a compatible cloud model or start with AI-free recognition. “Saved/configured” does not mean a server is running.

Choose a genuinely downloaded local model if you want local inference; a cloud model forwarded by the local service is still a cloud service. Online research still accesses public pages and Tavily and may use search quota.

### Existing Bailian / DeepSeek settings

“原有官方提供商” retains the original configuration within the same installation identity, not a cross-device key migration or a guarantee that upgrade installation has been accepted. Company research prefers Bailian web research, with explicitly marked **non-web DeepSeek analysis** as its fallback. Do not treat that fallback as current, sourced risk research.

For job web completion and company risk research, **this version's built-in official route permits only `deepseek-v4-pro`** through `/responses`; it never falls back to Bailian. The default `deepseek-v4-flash` is rejected for this route, and the app does not automatically upgrade to Pro. To use it, deliberately select Pro in the original DeepSeek settings, save/test, and check that job/risk tasks still use the original route. This describes the app's guard, not a claim that every current provider capability was live-tested.

Pasted-text extraction does not search: the original route can use configured DeepSeek Flash or Pro, but Bailian alone cannot perform it. Alternatively, a custom compatible model plus Tavily can research online. Adding DeepSeek as a custom model uses that Tavily route and does not inherit the original provider key or built-in search. A single official Responses request may involve multiple server-side searches, so one click is not a fixed billing unit. See [DeepSeek's Responses documentation](https://api-docs.deepseek.com/api/create-response/).

Android implements these routes too. Cancellation or model/search timeouts stop the task without starting another provider; implementation is not a substitute for real-device or live-provider acceptance.

## 4. Review results and explicitly save

For online completion, create the basic application first. If automatic research is not enabled, open the job and click “开始联网补全”. Verify company, role, city, evidence, and source links. Only supported empty fields may be prefilled in a draft; conflicts are not selected by default. Shared company-field changes affect other jobs at that company.

Add chosen suggestions to the editable draft with **加入可编辑草稿**, then click **保存全部更改** to commit them. Closing the suggestion panel does not save or undo draft changes. The app does not let AI decide stages, priorities, contacts, reminders, outcomes, or personal notes.

For a page you cannot read, choose **粘贴招聘原文** (Paste job description):

1. Paste text for one company and role, up to **50,000 characters**. Remove names, phone numbers, email addresses, résumé contents, and other private information.
2. Check the actual job model, accept the privacy/cost notice, and run extraction. It uses the saved job model only; no Tavily call, link opening, search, or provider fallback is performed.
3. Every suggestion starts **unchecked**. Review the original-text evidence, choose items, add them to the draft, and explicitly save.

These results are labeled “User-provided job description, not verified online”. They only suggest evidence-supported job and compensation fields, not company-wide data or risk assessments. The complete pasted text stays in the current window's memory; **accepted fields and limited evidence excerpts can persist in drafts, records, and JSON backups**.

## 5. Check a saved setup and troubleshoot

**AI 一键检查** checks the saved job-completion route, not every task or provider. Save your model and search settings first. Missing configuration can be checked locally without sending requests. With complete configuration, accept the cost notice before running the online check. It performs at most one model test and one corresponding search test in sequence, using fixed test text rather than your applications. A failure stops the check without automatic retries or fallback.

| Problem | What to check |
| --- | --- |
| Model saved, but shown as unused | Default and task assignments; saving alone does not enable it |
| Model connects, search fails | Tavily credentials/quota, or the selected original provider's search |
| DeepSeek Flash can analyze text but cannot research online | Select Pro explicitly for the built-in job/risk route, or use a compatible profile＋Tavily; there is no automatic model upgrade |
| Android cannot reach the PC's Ollama | Phone loopback is not the PC, and LAN addresses are not accepted by this local route; use a cloud model or AI-free recognition |
| Authentication, rate-limit, or balance error | The relevant service's key, model access, quota, and billing |
| Missing sources or inaccessible job page | Correct company/city/public link, or extract pasted text instead |
| Invalid structured output | Whether that exact service and model support the required format |

Stopping a request prevents further local work but cannot reverse charges for work already processed by a provider. Closing details or switching records cancels the active request; moving between tabs of the same detail does not. On Android, leaving the foreground also cancels active and queued AI network tasks. Keep the app in the foreground while waiting; do not expect background completion.

Windows uses Electron secure storage; Android uses Android Keystore to encrypt key configuration. Model/search keys are excluded from job-data IndexedDB and JSON backups, so configure them yourself on a new device. Online research uses only required company/job identity fields and safely retrieved public text, not contacts, personal notes, interview history, or attachments. Cloud text extraction sends the text you choose to paste: remove sensitive information first, and do not put private details in research identity fields or URLs. Ordinary records, drafts, and backups are not an encrypted vault.

AI behavior has automated coverage with simulated responses; complete paid end-to-end checks against every real provider have not been performed. Android AI, system key storage, foreground/background transitions and service reachability also remain unaccepted on a real phone. Implemented native routes do not establish support on every phone or model. Actual connectivity, quotas, and output quality need your own verification. AI failure does not disable local records.

[Privacy, in Chinese](../../PRIVACY.md) · [Report an issue without keys or private data](https://github.com/YCC-Lover/Offer-King/issues/new?template=bug_report.yml)

### Updates are notifications, not automatic installation

Windows 2.5.4 can check at startup and during foreground use, at most once per day automatically; manual checks are also available. Settings let you turn off automatic checking, include/exclude candidates, or ignore a version. It reads this project's official GitHub release metadata and only notifies for a newer version with a matching platform asset. **It does not download or install automatically**, and it is not a system background push service.

Android has a native checker, but this development-signed `Offer-King-2.5.4-android-trial.apk` is not a formal Android update-matching asset. Get it manually from the [2.5.4 release page](https://github.com/YCC-Lover/Offer-King/releases/tag/v2.5.4); do not expect automatic delivery or compatibility with a differently signed installation. Older versions without a checker need manual downloading. GitHub Watch Releases notifications depend on GitHub account settings, not the app.

Read `START-HERE.md` and verify the checksum first; back up JSON and keep original attachments before any upgrade. Do not disable security protection to bypass warnings or uninstall an Android app merely to bypass a signature mismatch. Share only the release page and guide, never your data directory, backups or keys.

Updated 2026-10-19 for the 2.5.4 candidate. Provider policies and charges are governed by the providers' current terms.
