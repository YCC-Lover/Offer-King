# Download Offer King

[简体中文](../../DOWNLOAD.md) · [English](DOWNLOAD.md) · [日本語](../ja/DOWNLOAD.md) · [한국어](../ko/DOWNLOAD.md)

[English home](README.md) · [AI setup](AI-SETUP.md)

## 2.6.0 candidate trial downloads

**[Windows 10 / 11 x64 trial · EXE](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.0/Offer-King-Setup-2.6.0.exe)** · **[Android development trial · APK](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.0/Offer-King-2.6.0-android-trial.apk)**

Windows: **112,107,822 bytes**. Android: **33,734,163 bytes**.

[Fixed v2.6.0 release page](https://github.com/YCC-Lover/Offer-King/releases/tag/v2.6.0) · [SHA256SUMS.txt](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.0/SHA256SUMS.txt) · [START-HERE.md](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.0/START-HERE.md) · [TEST-RESULTS.json](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.0/TEST-RESULTS.json)

> **Limited trial candidate (Pre-release), not a production release.** Windows has no production code signature (**NotSigned**). Android uses a **Debug development/test signature**, not a production identity. Windows clean/upgrade installation and uninstallation, and Android real-device first installation, upgrade and runtime use, have **not completed acceptance testing**. Back up before upgrading. [Verification scope, in Chinese](../../RELEASE-2.6.0.md)

These are the five release assets: the Windows EXE, Android APK, checksum list, starting guide and test-results summary. Public downloads do not require a GitHub account. Choose the file for your device; GitHub's `Source code` archives contain this public repository's documentation and cannot install the app. No developer tools are needed.

## Requirements and first use

- **Windows:** Windows 10 / 11, x64; minimum window 1100 × 700.
- **Android:** development trial APK, minimum Android 7.0 / API 24; real-device compatibility and first/upgrade installation remain unaccepted. The Windows 1100 × 700 limit does **not** apply to Android.
- There are **no macOS, iOS or Linux installers**. Font size is adjustable from 90% to 125%; this does not establish every phone's layout compatibility.
- Local application management works without an app account, AI account, or internet connection. Optional AI uses your own configuration and may incur charges.
- New users start with an empty database. The installer contains no personal applications or shared API keys.

After installation, choose a language in the sidebar or Settings & backup → Display & readability, then use Add application to create a record. Language changes apply immediately without clearing current input; your own company names, job titles, notes, and custom stages are not translated. [Getting started, in Chinese](../../QUICKSTART.md)

### Local tools in 2.6.0

**New in 2.6.0:** local quick find (`Ctrl/Cmd + K`), board/list views, combined filters, up to 12 named views and quick follow-up work without AI. Quick follow-up requires an explicit Save and records the change without changing the application stage. The compact home, expandable detail sections and mobile large-text layout are also improved. [Full release notes](../../RELEASE-2.6.0.md)

- **Paste instead of retyping:** Add application now has an offline recognition preview. Review evidence and fill only selected empty fields; existing input is not overwritten. The full text stays in the current window's memory and is not included in recovery drafts or backups. No AI setup, network request, or AI fee is involved.
- **Take-home pay:** estimate CNY salary, employee contributions and income tax for a mainland Chinese resident with 12 fixed monthly payments from the same employer starting in January. Any city can use custom bases/rates; Beijing's reference template requires an explicit Apply action. The estimate never changes the original job or city budget, does not convert foreign pay, and is not tax advice. Calculation is offline and free of AI fees.

## What was verified

1,280 unit/component tests passed; Node tests had 314 passes and 4 skips. Five packaged Electron scenarios and one unpacked 2.5.4 → 2.6.0 upgrade scenario with synthetic data passed. Android was compiled, signed with the existing Debug certificate, and checked for package structure, version, assets and signature. Responsive browser/touch checks covered large text.

**This does not establish real installation acceptance.** Windows clean installation, installer-based upgrade and uninstallation, and Android real-device installation, upgrade, permissions, keyboard and runtime behavior are still unaccepted. No production signing identity, macOS/iOS package or live paid AI test is included. [Test report, in Chinese](../../RELEASE-2.6.0.md#已验证与尚未验收)

## Check the downloaded file

On Windows, open PowerShell in the folder containing the downloaded files and run the applicable command:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath '.\Offer-King-Setup-2.6.0.exe'
Get-FileHash -Algorithm SHA256 -LiteralPath '.\Offer-King-2.6.0-android-trial.apk'
```

Windows EXE — **112,107,822 bytes**, SHA-256:

```text
495A394BC9FD565CF18120A469C3EDA145463F2C52D32A0901028E492320FEFE
```

Android APK — **33,734,163 bytes**, SHA-256:

```text
5BC13988FCA751CEF0E3477E672C0459B6A55FF1FFF336BF516EB50ADB37518E
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
3. This APK reuses the earlier development trial's Debug signer. Matching app ID and signature are only static prerequisites, **not proof that an in-place upgrade works**. This build is version 2.6.0 (version code 2006000); its hash identifies the exact file.
4. If you see a signature conflict, version error or security block, **stop and report it; do not simply uninstall the old app or clear its data**. A future production signer may not replace this Debug build directly. Do not use uninstalling as a migration plan.
5. Start with fictional records and AI unconfigured. Check offline creation, save/reopen, JSON export, 125% text, scrolling and document authorization. These real-device checks are still pending; a successful build is not a successful device test.

## Release notifications are not automatic installation

With automatic checks enabled, **Windows 2.5.4 and later can check once per day while the app is open and foregrounded**, or you can check manually. When upgrading from an older version, enable **Include candidate releases** to receive the 2.6.0 notice. The app opens the official release page on request; it does not download or install the update. Users on **2.4.0 or earlier must upgrade manually once** to receive the new notification feature. GitHub Watch is a separate service.

The **Android Debug trial is not recommended as a production auto-update channel**. Follow the fixed release and backup instructions manually. GitHub's Latest label may point elsewhere; use the v2.6.0 links above. Share only the APK/EXE and guides, never personal data folders, backups or keys.

[AI setup](AI-SETUP.md) · [Privacy, in Chinese](../../PRIVACY.md) · [Feedback](../../../CONTRIBUTING.md)

Download information updated 2026-10-23.
