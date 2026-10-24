# Download Offer King

[简体中文](../../DOWNLOAD.md) · [English](DOWNLOAD.md) · [日本語](../ja/DOWNLOAD.md) · [한국어](../ko/DOWNLOAD.md)

[English home](README.md) · [AI setup](AI-SETUP.md)

## Android 2.6.1 / Windows 2.6.0 candidate trial downloads

**[Windows 10 / 11 x64 · 2.6.0 EXE](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.0/Offer-King-Setup-2.6.0.exe)** · **[Android development trial · 2.6.1 APK](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.1/Offer-King-2.6.1-android-trial.apk)**

Windows 2.6.0: **112,107,822 bytes**. Android 2.6.1: **33,735,427 bytes**. This release changes Android only; there is no new Windows installer.

[Android v2.6.1 release](https://github.com/YCC-Lover/Offer-King/releases/tag/v2.6.1) · [Android SHA256SUMS.txt](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.1/SHA256SUMS.txt) · [Android START-HERE.md](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.1/START-HERE.md) · [Android TEST-RESULTS.json](https://github.com/YCC-Lover/Offer-King/releases/download/v2.6.1/TEST-RESULTS.json) · [Windows v2.6.0 release and verification files](https://github.com/YCC-Lover/Offer-King/releases/tag/v2.6.0)

> **Limited trial candidates (Pre-release), not production releases.** Windows has no production code signature (**NotSigned**). Android uses a **Debug development/test signature**, not a production identity. Windows clean/upgrade installation and uninstallation, and Android real-device first installation, in-place upgrade, encrypted AI-key retention and runtime use, have **not completed acceptance testing**. Back up before upgrading. [Android verification scope, in Chinese](../../RELEASE-2.6.1.md)

The Android 2.6.1 release provides its APK, checksum list, starting guide and test-results summary; Windows remains in the separate 2.6.0 release. Public downloads do not require a GitHub account. Choose the file for your device; GitHub's `Source code` archives contain this public repository's documentation and cannot install the app. No developer tools are needed.

## Requirements and first use

- **Windows:** Windows 10 / 11, x64; minimum window 1100 × 700.
- **Android:** development trial APK, minimum Android 7.0 / API 24; real-device compatibility and first/upgrade installation remain unaccepted. The Windows 1100 × 700 limit does **not** apply to Android.
- There are **no macOS, iOS or Linux installers**. Font size is adjustable from 90% to 125%; this does not establish every phone's layout compatibility.
- Local application management works without an app account, AI account, or internet connection. Optional AI uses your own configuration and may incur charges.
- New users start with an empty database. The installer contains no personal applications or shared API keys.

After installation, choose a language in the sidebar or Settings & backup → Display & readability, then use Add application to create a record. Language changes apply immediately without clearing current input; your own company names, job titles, notes, and custom stages are not translated. [Getting started, in Chinese](../../QUICKSTART.md)

### New Android update reminders, existing local tools

**Android 2.6.1:** recognize official future trial APKs, check manually or automatically in the foreground at most once per 24 hours when enabled, and open the official release page. Candidate-release and ignored-version preferences apply. Downloads and installation stay manual; dark-mode update notices have clearer text. Checking releases makes no AI calls and sends no company records or keys. [2.6.1 notes](../../RELEASE-2.6.1.md)

**New in 2.6.0:** local quick find (`Ctrl/Cmd + K`), board/list views, combined filters, up to 12 named views and quick follow-up work without AI. Quick follow-up requires an explicit Save and records the change without changing the application stage. The compact home, expandable detail sections and mobile large-text layout are also improved. [Full release notes](../../RELEASE-2.6.0.md)

- **Paste instead of retyping:** Add application now has an offline recognition preview. Review evidence and fill only selected empty fields; existing input is not overwritten. The full text stays in the current window's memory and is not included in recovery drafts or backups. No AI setup, network request, or AI fee is involved.
- **Take-home pay:** estimate CNY salary, employee contributions and income tax for a mainland Chinese resident with 12 fixed monthly payments from the same employer starting in January. Any city can use custom bases/rates; Beijing's reference template requires an explicit Apply action. The estimate never changes the original job or city budget, does not convert foreign pay, and is not tax advice. Calculation is offline and free of AI fees.

## What was verified

Android 2.6.1 passed 1,291 unit/component tests, 110 native JVM checks, 27 native-contract tests and 6 simulated browser scenarios, along with type/lint checks and independent APK verification. It was rebuilt with the existing Debug certificate; these checks do not demonstrate a real phone upgrade. See the [2.6.1 test scope](../../RELEASE-2.6.1.md) and attached test-results summary.

For the previous 2.6.0 release, 1,280 unit/component tests passed; Node tests had 314 passes and 4 skips. Five packaged Electron scenarios and one unpacked 2.5.4 → 2.6.0 upgrade scenario with synthetic data passed. Those are historical results, not new 2.6.1 installation evidence.

**This does not establish real installation acceptance.** Windows clean installation, installer-based upgrade and uninstallation, and Android real-device installation, upgrade, permissions, keyboard and runtime behavior are still unaccepted. No production signing identity, macOS/iOS package or live paid AI test is included. [Test report, in Chinese](../../RELEASE-2.6.0.md#已验证与尚未验收)

## Check the downloaded file

On Windows, open PowerShell in the folder containing the downloaded files and run the applicable command:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath '.\Offer-King-Setup-2.6.0.exe'
Get-FileHash -Algorithm SHA256 -LiteralPath '.\Offer-King-2.6.1-android-trial.apk'
```

Windows EXE — **112,107,822 bytes**, SHA-256:

```text
495A394BC9FD565CF18120A469C3EDA145463F2C52D32A0901028E492320FEFE
```

Android 2.6.1 APK — **33,735,427 bytes**, SHA-256:

```text
13314462F858E6DC88D834030D3CCCE8C766BE57D42AC43A1F73EDE0078E789F
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

1. If an older app is installed, explicitly save pending edits, export JSON **outside the app's own storage**, and confirm the file exists. Keep attachment originals separately. JSON excludes API keys and attachment files; it cannot restore keys after uninstalling.
2. Download and verify the 2.6.1 APK, then open it with the phone's system file manager and select **Update** over the existing app. Keep the app installed; do not clear data or reset AI settings to prepare for this upgrade. Follow system security guidance without disabling Play Protect or other protection.
3. This APK reuses the 2.6.0 Debug signer, app ID `com.offerflow.mobile`, data origin and AI secure-storage configuration. They are designed to preserve existing records and AI configuration during an in-place update, **not proof of successful device upgrade or key retention**. This build is version 2.6.1 (version code 2006001); its hash identifies the exact file. After reopening, check records, attachment access and AI configuration status before making changes; keeping configuration does not require a paid AI test.
4. If you see a signature conflict, version error or security block, **stop and report it; do not simply uninstall the old app or clear its data**. A future production signer may not replace this Debug build directly. Do not use uninstalling as a migration plan.
5. On a fresh trial installation, start with fictional records and AI unconfigured. Check offline creation, save/reopen, JSON export, 125% text, scrolling and document authorization. **Real-phone first installation, in-place upgrade and Android Keystore continuity are still unaccepted**; a successful build is not a successful device test.

## Release notifications are not automatic installation

With automatic checks enabled, **Windows 2.5.4 and later can check once per day while the app is open and foregrounded**, or you can check manually. When upgrading from an older version, enable **Include candidate releases** to receive the 2.6.0 notice. The app opens the official release page on request; it does not download or install the update. Users on **2.4.0 or earlier must upgrade manually once** to receive the new notification feature. GitHub Watch is a separate service.

**Android trial 2.6.0 and earlier must be upgraded to 2.6.1 manually once:** the old checker does not match trial APK filenames, even with a manual check. In 2.6.1, open **Help & about → App updates**, enable candidate releases, and choose Check for updates. Automatic checks run while foregrounded at most once per 24 hours when enabled; ignored versions stay ignored until restored. Only a higher official matching release is offered. The button opens the official release page; it does not fetch/install an APK or guarantee compatibility with a future production signer. Update checks do not call AI or change its settings.

GitHub's Latest label may point elsewhere; use the Android v2.6.1 and Windows v2.6.0 links above. Share only the APK/EXE and guides, never personal data folders, backups or keys.

[AI setup](AI-SETUP.md) · [Privacy, in Chinese](../../PRIVACY.md) · [Feedback](../../../CONTRIBUTING.md)

Download information updated 2026-10-24.
