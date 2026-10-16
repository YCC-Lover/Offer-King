# Offer King AI setup

[简体中文](../../AI-SETUP.md) · [English](AI-SETUP.md) · [日本語](../ja/AI-SETUP.md) · [한국어](../ko/AI-SETUP.md)

[English home](README.md) · [Download](DOWNLOAD.md) · [Detailed Chinese guide](../../AI-SETUP.md)

This guide describes the **2.3.0 candidate release**. Switch between Simplified Chinese, English, Japanese, and Korean in the sidebar or display settings; switching preserves current input and takes effect immediately. The installer is unsigned (NotSigned); real clean installation, upgrade installation, and uninstallation have not yet completed acceptance testing. [Download and verification](DOWNLOAD.md)

The steps below include Chinese labels in addition to English descriptions so they can also be followed with older screenshots. Interface language changes do not translate your records or change your AI provider, key, model, search route, or billing consent.

You can manage applications, tasks, offers, and backups without AI. AI is optional, uses your own accounts and keys, and may consume quota or incur charges. **No shared key or unlimited free service is included.**

## 1. Choose the task first

| What you want | Configuration needed | Web search? |
| --- | --- | --- |
| Extract fields from a job description you paste | Compatible job model, or a prepared local Ollama model | No; Tavily is not required |
| Research public company or job information | Compatible model plus your Tavily key, or the existing provider route | Yes; review the sources |
| Keep local records, tasks, comparisons, and backups | None | No AI calls |

Text extraction **does not verify the description online**. A successful model connection does not establish that search or structured extraction will work.

## 2. Free-start preset

1. Open **设置与备份 → AI 调研 → 免费 AI 起步** (Settings & backup → AI research → Free AI start).
2. Create your own key at [OpenRouter](https://openrouter.ai/settings/keys) and enter it in “OpenRouter 免费模型 API Key”. The preset uses `openrouter/free` at `https://openrouter.ai/api/v1`.
3. Obtain your own search key from [Tavily](https://app.tavily.com/home) and enter “免费起步 Tavily API Key”. Check both services' current quotas and billing settings if you intend to stay within free allowances.
4. Click **保存并启用免费配置** (Save and enable free configuration). This explicitly switches company, job, and risk tasks to the preset; saving alone does not start research.
5. Run the model and search tests, or use the one-click check after reading the cost notice. Tests may use quota.

Free model availability and provider allowances can change; the app does not promise a fixed quota or permanent free use. It does not silently replace a failed free model with a paid model. Provider-side billing settings remain your responsibility.

“创建岗位后自动调研” (Research automatically after creating a job) is **off by default**. To opt in, enable it and click “保存自动调研偏好”. It runs once after a new application is successfully created, not while typing and not automatically for old applications.

## 3. Use your own model

Open **我的模型配置 → 新增模型配置** (My model configurations → Add configuration). Enter a recognizable name, protocol, base URL, exact model ID, and the corresponding API key. Supported routes include OpenAI-compatible Chat Completions, Responses, and local Ollama; the service/model must support the structured output the app requires. A chat website subscription does not necessarily include API access.

Cloud endpoints must be public HTTPS addresses. Check the normalized base address before saving. Read model IDs with “读取模型列表” or enter an exact ID manually if listing is unavailable.

**Saving a model does not enable it.** Test the saved model, then choose “设为默认并保存” or save the desired default/task assignments. Separate task overrides continue to apply; check the model card's actual scope. When changing service endpoints or protocols, provide the key for the new service.

For online research with compatible models, save and test your key in **联网搜索 · Tavily**. Text-only extraction does not need it. Advanced settings can assign separate models to company, job, and risk tasks. A failed selected route is reported rather than silently switching to another paid service.

### Local Ollama

Install and run Ollama yourself and download a suitable local model. Choose “Ollama 本机模型”; the default endpoint is `http://127.0.0.1:11434/v1`, and no API key is needed. The app connects only to the local loopback service and does not install Ollama or download models for you.

Choose a genuinely downloaded local model if you want local inference; a cloud model forwarded by the local service is still a cloud service. Online research still accesses public pages and Tavily and may use search quota.

### Existing Bailian / DeepSeek settings

“原有官方提供商” retains the original route. Company research prefers Bailian web research, with explicitly marked non-web DeepSeek analysis as its fallback. Job web completion and company risk research use DeepSeek's official online route, without Bailian fallback. Pasted job-text extraction on that original job route requires DeepSeek; Bailian alone cannot perform it.

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
| Authentication, rate-limit, or balance error | The relevant service's key, model access, quota, and billing |
| Missing sources or inaccessible job page | Correct company/city/public link, or extract pasted text instead |
| Invalid structured output | Whether that exact service and model support the required format |

Stopping a request prevents further local work but cannot reverse charges for work already processed by a provider. Closing details or switching records cancels the active request; moving between tabs of the same detail does not.

Keys are encrypted locally and excluded from job-data IndexedDB and JSON backups. Online research uses only required company/job identity fields and safely retrieved public text, not contacts, personal notes, interview history, or attachments. Cloud text extraction sends exactly the text you choose to paste: remove sensitive information first. Ordinary records, drafts, and backups are not an encrypted vault.

AI behavior has automated coverage with simulated responses; complete paid end-to-end checks against every real provider have not been performed. Actual connectivity, quotas, and output quality need your own verification. AI failure does not disable local records.

[Privacy, in Chinese](../../PRIVACY.md) · [Report an issue without keys or private data](https://github.com/YCC-Lover/Offer-King/issues/new?template=bug_report.yml)

Updated 2026-10-16 for the 2.3.0 candidate. Provider policies and charges are governed by the providers' current terms.
