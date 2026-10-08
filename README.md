<p align="center">
  <img src="logo.png" alt="WannaFlix VPN" width="180">
</p>

<h1 align="center">WannaFlix Beta</h1>

<p align="center">
  Public beta builds of <strong>WannaFlix VPN</strong><br>
  for customer testing before wider release.
</p>

<p align="center">
  <img alt="Beta" src="https://img.shields.io/badge/Status-Public%20Beta-c41e3a?style=for-the-badge">
</p>

---

## What is WannaFlix VPN?

**WannaFlix VPN** is a multi-platform VPN client. Sign in with your WannaFlix access token, download the server list, and connect through the app on Android, Windows, and macOS.

This repository does **not** contain application source code. It exists so we can publish **public beta installers** and collect feedback from customers who want to try new builds early.

### Relationship to FlClash

WannaFlix VPN is a modified version of [FlClash](https://github.com/chen08209/FlClash), an open-source multi-platform proxy client based on Clash.Meta (mihomo), licensed under **GPL-3.0**.

Original FlClash copyright notices are retained. The FlClash authors do **not** publish WannaFlix builds and are not responsible for this product.

---

## Getting a beta build

1. Open the **Releases** page on this GitHub repository.
2. Download the installer for your platform from the latest (or a specific) beta tag.
3. Install or replace your current WannaFlix build with the beta package.
4. Sign in with your usual WannaFlix access token.

Typical artifacts (names vary by version):

| Platform | What to download |
| --- | --- |
| **Android** | `WannaFlix-*-android-arm64-v8a.apk` (most phones) |
| **Windows (x64)** | `WannaFlix-*-windows-amd64-setup.exe` |
| **Windows (ARM64)** | `WannaFlix-*-windows-arm64-setup.exe` |
| **macOS (Apple Silicon)** | `WannaFlix-*-macos-arm64.dmg` |

Always prefer the file that matches your device architecture. When in doubt on Android phones, use **arm64-v8a**.

> **Note:** Beta builds may be unsigned or signed differently from production. On Android you may need to allow installs from unknown sources. On Windows or macOS you may need to approve a security prompt the first time you open the app.

---

## Beta testing guidelines

Thank you for helping improve WannaFlix. Useful feedback is specific, reproducible, and tied to a build version.

### Before you start

- Note the **exact release tag** or file name you installed (for example `WannaFlix-0.1.02-…`).
- Write down your **OS version** (Android / Windows / macOS) and device type.
- If possible, test on a device you can reset or where a broken VPN setup will not block critical work.

### What to try

- First launch and sign-in with your access token
- Connecting, disconnecting, and reconnecting
- Switching servers or modes (if available in the build)
- App behavior after sleep, reboot, or network changes (Wi‑Fi ↔ cellular)
- Upgrade from a previous beta or stable build, when applicable

### What to report

Please report problems in this repository’s **Issues** tab (or the channel your WannaFlix contact specified), and include:

1. **Build** — release tag or exact installer / APK file name  
2. **Device** — OS, version, and architecture (e.g. Windows 11 ARM64, Android 14 arm64)  
3. **Steps** — what you did, in order  
4. **Expected vs actual** — what should have happened, what happened instead  
5. **Screenshots or short screen recordings** when the UI is involved  
6. **Relevant logs** if you can capture them (see below)  
7. **Workarounds** you already tried (reinstall, new token, reboot, etc.)

### Good bug titles

- `Windows ARM64: app crashes when enabling TUN after sleep`
- `Android: sign-in accepts token but server list stays empty`
- `macOS: DMG opens but app is blocked on first launch`

Avoid vague titles like “doesn’t work” or “bug”.

### Regression and change notes

If something worked in an earlier beta and failed after updating:

- Name **both** versions (old → new)
- Say whether a clean install vs upgrade made a difference
- Mention any setting you changed between builds

Positive notes are welcome too: “connects faster on Wi‑Fi than 0.1.01” helps as much as a crash report.

### Logs and privacy

- Prefer logs from the session where the problem occurred.
- **Do not** paste your WannaFlix access token, passwords, or other account secrets into a public issue.
- Redact personal identifiers from screenshots when possible.

---

## Known expectations for beta software

- Features and UI may change between betas without a long migration path.
- A beta can be less stable than the build you use day to day.
- We may yank or replace a release if a serious issue is found.
- Feedback may be grouped; not every report will get an individual reply, but it is reviewed.

If a beta leaves you unable to connect, install the previous release from **Releases** or your last known-good package until a fix is published.

---

## Support and community

- **Beta downloads:** the **Releases** page on this repository
- **Bug reports / feedback:** the **Issues** tab on this repository
- **WannaFlix Telegram:** [Join the channel](https://telegram.me/+8_vEJYAkTXlhYzA1)

For account or subscription questions that are not about a beta build, contact WannaFlix support through your usual channel rather than filing a GitHub issue.

---

## License and attribution

WannaFlix VPN builds distributed here are based on FlClash and related open-source components.

- FlClash: [github.com/chen08209/FlClash](https://github.com/chen08209/FlClash) (GPL-3.0)
- Clash.Meta / mihomo and other third-party components follow their own licenses

This repository is for **beta distribution and feedback** only. Source for the modified application is provided separately under the applicable open-source licenses where required.
