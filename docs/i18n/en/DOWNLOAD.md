# Download Offer King

[简体中文](../../DOWNLOAD.md) · [English](DOWNLOAD.md) · [日本語](../ja/DOWNLOAD.md) · [한국어](../ko/DOWNLOAD.md)

[English home](README.md) · [AI setup](AI-SETUP.md)

## Windows download

**[Download 2.4.0 candidate · Windows 10 / 11 x64](https://github.com/YCC-Lover/Offer-King/releases/download/v2.4.0/Offer-King-Setup-2.4.0.exe)**

Size: **111,979,180** bytes (**106.8 MiB**) · [Release page](https://github.com/YCC-Lover/Offer-King/releases/tag/v2.4.0) · [Checksum file](https://github.com/YCC-Lover/Offer-King/releases/download/v2.4.0/SHA256.txt) · [Offline introduction](https://github.com/YCC-Lover/Offer-King/releases/download/v2.4.0/START-HERE.txt)

> This unsigned **2.4.0 candidate (Pre-release / NotSigned)** includes Simplified Chinese, English, Japanese, and Korean. Real clean installation, installation over an existing version, and uninstallation have **not yet completed acceptance testing**. [Verification scope, in Chinese](../../RELEASE-2.4.0.md#已验证与尚未验收)

Public downloads do not require a GitHub account. Download the `.exe`; GitHub's `Source code` archives contain this public repository's documentation and cannot install the app. No developer tools are needed.

## Requirements and first use

- Windows 10 / 11, x64. No macOS, Linux, or mobile installer is available.
- Minimum window size: 1100 × 700. Font size can be adjusted from 90% to 125% in settings.
- Local application management works without an app account, AI account, or internet connection. Optional AI uses your own configuration and may incur charges.
- New users start with an empty database. The installer contains no personal applications or shared API keys.

After installation, choose a language in the sidebar or Settings & backup → Display & readability, then use Add application to create a record. Language changes apply immediately without clearing current input; your own company names, job titles, notes, and custom stages are not translated. [Getting started, in Chinese](../../QUICKSTART.md)

### New local tools in 2.4.0

- **Paste instead of retyping:** Add application now has an offline recognition preview. Review evidence and fill only selected empty fields; existing input is not overwritten. The full text stays in the current window's memory and is not included in recovery drafts or backups. No AI setup, network request, or AI fee is involved.
- **Take-home pay:** estimate CNY salary, employee contributions and income tax for a mainland Chinese resident with 12 fixed monthly payments from the same employer starting in January. Any city can use custom bases/rates; Beijing's reference template requires an explicit Apply action. The estimate never changes the original job or city budget, does not convert foreign pay, and is not tax advice. Calculation is offline and free of AI fees.

## Check the downloaded file

Open PowerShell in the folder containing the installer and run:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath '.\Offer-King-Setup-2.4.0.exe'
```

The file size should be **111,979,180** bytes, and SHA-256 should be:

```text
0670A784B88C53B51C959350012A3894428F5E561BB74D27DC8820200191604D
```

A matching hash confirms that the file matches this release; it is not a digital signature or a security certification. Use the corresponding release's values for other versions.

An unsigned installer may trigger “Unknown publisher” or SmartScreen. Check the download source and follow Windows security guidance. Do not disable Defender, SmartScreen, or other protection. If you cannot verify the file or it remains blocked, stop and [report the issue](https://github.com/YCC-Lover/Offer-King/issues/new?template=bug_report.yml).

## Upgrading an existing installation

1. In the old app, manually export a JSON backup from “设置与备份”. Keep the original attachment files separately.
2. Close the app and keep its existing installation location. Do not clear app data to prepare for an update.
3. If you accept the candidate-build limitations, run the installer. After launch, check your companies, applications, and AI configuration status. Keep the pre-upgrade backup.
4. If something is wrong, preserve the current state and report it before clearing data or importing over unchecked records.

The release is designed to retain installation identity and data location. See the release notes for the verification scope; automated checks do not establish real installer upgrade acceptance. JSON backups exclude API keys, unsaved drafts, and attachment files. On another computer, move attachment originals separately and configure your own AI keys again.

There is **no automatic updater or in-app release push**. Visit the release page and download an update manually after reading its notes and backing up. GitHub's Latest label may point to another release; use the fixed 2.4.0 links above for this candidate. Share this page, the installer, and the guide with friends—not personal data folders, backups, or keys.

[AI setup](AI-SETUP.md) · [Privacy, in Chinese](../../PRIVACY.md) · [Feedback](../../../CONTRIBUTING.md)

Download information checked 2026-10-18.
