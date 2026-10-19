# Download Offer King

[简体中文](../../DOWNLOAD.md) · [English](DOWNLOAD.md) · [日本語](../ja/DOWNLOAD.md) · [한국어](../ko/DOWNLOAD.md)

[English home](README.md) · [AI setup](AI-SETUP.md)

## 2.5.4 candidate trial downloads

**[Windows 10 / 11 x64 trial · EXE](https://github.com/YCC-Lover/Offer-King/releases/download/v2.5.4/Offer-King-Setup-2.5.4.exe)** · **[Android development trial · APK](https://github.com/YCC-Lover/Offer-King/releases/download/v2.5.4/Offer-King-2.5.4-android-trial.apk)**

Windows: **112,083,805 bytes**. Android: **33,702,975 bytes**.

[Fixed v2.5.4 release page](https://github.com/YCC-Lover/Offer-King/releases/tag/v2.5.4) · [SHA256SUMS.txt](https://github.com/YCC-Lover/Offer-King/releases/download/v2.5.4/SHA256SUMS.txt) · [START-HERE.md](https://github.com/YCC-Lover/Offer-King/releases/download/v2.5.4/START-HERE.md) · [TEST-RESULTS.json](https://github.com/YCC-Lover/Offer-King/releases/download/v2.5.4/TEST-RESULTS.json)

> **Limited trial candidate (Pre-release), not a production release.** Windows has no production code signature (**NotSigned**). Android uses a **Debug development/test signature**, not a production identity. Windows clean/upgrade installation and uninstallation, and Android real-device first installation, upgrade and runtime use, have **not completed acceptance testing**. Back up before upgrading. [Verification scope, in Chinese](../../RELEASE-2.5.4.md)

These are the five release assets: the Windows EXE, Android APK, checksum list, starting guide and test-results summary. Public downloads do not require a GitHub account. Choose the file for your device; GitHub's `Source code` archives contain this public repository's documentation and cannot install the app. No developer tools are needed.

## Requirements and first use

- **Windows:** Windows 10 / 11, x64; minimum window 1100 × 700.
- **Android:** development trial APK, minimum Android 7.0 / API 24; real-device compatibility and first/upgrade installation remain unaccepted. The Windows 1100 × 700 limit does **not** apply to Android.
- There are **no macOS, iOS or Linux installers**. Font size is adjustable from 90% to 125%; this does not establish every phone's layout compatibility.
- Local application management works without an app account, AI account, or internet connection. Optional AI uses your own configuration and may incur charges.
- New users start with an empty database. The installer contains no personal applications or shared API keys.

After installation, choose a language in the sidebar or Settings & backup → Display & readability, then use Add application to create a record. Language changes apply immediately without clearing current input; your own company names, job titles, notes, and custom stages are not translated. [Getting started, in Chinese](../../QUICKSTART.md)

### Local tools retained in 2.5.4

- **Paste instead of retyping:** Add application now has an offline recognition preview. Review evidence and fill only selected empty fields; existing input is not overwritten. The full text stays in the current window's memory and is not included in recovery drafts or backups. No AI setup, network request, or AI fee is involved.
- **Take-home pay:** estimate CNY salary, employee contributions and income tax for a mainland Chinese resident with 12 fixed monthly payments from the same employer starting in January. Any city can use custom bases/rates; Beijing's reference template requires an explicit Apply action. The estimate never changes the original job or city budget, does not convert foreign pay, and is not tax advice. Calculation is offline and free of AI fees.

## Check the downloaded file

On Windows, open PowerShell in the folder containing the downloaded files and run the applicable command:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath '.\Offer-King-Setup-2.5.4.exe'
Get-FileHash -Algorithm SHA256 -LiteralPath '.\Offer-King-2.5.4-android-trial.apk'
```

Windows EXE — **112,083,805 bytes**, SHA-256:

```text
75B19B121A9736C2B46C62CCA9E40333B4F4E8E92528B34D4A10BBE4E4DE7A8D
```

Android APK — **33,702,975 bytes**, SHA-256:

```text
85CA9C2F67BE4EDE787016E6B9487D50F359C7171B271AFE8DFE022FECEAB89C
```

A matching hash confirms that the file matches this release; it is not a digital signature or a security certification. Use the corresponding release's values for other versions.

An unsigned installer may trigger “Unknown publisher” or SmartScreen. Check the download source and follow Windows security guidance. Do not disable Defender, SmartScreen, or other protection. If you cannot verify the file or it remains blocked, stop and [report the issue](https://github.com/YCC-Lover/Offer-King/issues/new?template=bug_report.yml).

## Upgrading Windows

1. In the old app, manually export a JSON backup from “设置与备份”. Keep the original attachment files separately.
2. Close the app and keep its existing installation location. Do not clear app data to prepare for an update.
3. If you accept the candidate-build limitations, run the installer. After launch, check your companies, applications, and AI configuration status. Keep the pre-upgrade backup.
4. If something is wrong, preserve the current state and report it before clearing data or importing over unchecked records.

The release is designed to retain installation identity and data location. See the release notes for the verification scope; automated checks do not establish real installer upgrade acceptance. JSON backups exclude API keys, unsaved drafts, and attachment files. On another device, keep attachment originals separately, reauthorize mobile documents when needed, and configure your own AI keys again. There is no automatic cross-device sync.

## Trying or upgrading Android

1. If an older app is installed, export a JSON backup and confirm it was saved before proceeding. Keep attachment originals separately.
2. Verify the APK and open it with the phone's system file manager, following its security guidance. Do not disable Play Protect or other system protections.
3. This APK reuses the earlier development trial's Debug signer. Matching app ID and signature are only static prerequisites, **not proof that an in-place upgrade works**. The version remains 2.5.4; the hash identifies this build.
4. If you see a signature conflict, version error or security block, **stop and report it; do not simply uninstall the old app or clear its data**. A future production signer may not replace this Debug build directly. Do not use uninstalling as a migration plan.
5. Start with fictional records and AI unconfigured. Check offline creation, save/reopen, JSON export, 125% text, scrolling and document authorization. These real-device checks are still pending; a successful build is not a successful device test.

## Release notifications are not automatic installation

With automatic checks enabled, **Windows 2.5.4 can check once per day while the app is open and foregrounded**, or you can check manually. The app opens the official release page on request; it does not download or install the update. Users on **2.4.0 or earlier must upgrade manually once** to receive the new notification feature. GitHub Watch is a separate service.

The **Android Debug trial is not recommended as a production auto-update channel**. Follow the fixed release and backup instructions manually. GitHub's Latest label may point elsewhere; use the v2.5.4 links above. Share only the APK/EXE and guides, never personal data folders, backups or keys.

[AI setup](AI-SETUP.md) · [Privacy, in Chinese](../../PRIVACY.md) · [Feedback](../../../CONTRIBUTING.md)

Download information updated 2026-10-19.
