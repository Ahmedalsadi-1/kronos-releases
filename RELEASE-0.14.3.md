# KronOS 0.14.3 public preview

KronOS is available as a public desktop preview for **Apple silicon Macs running
macOS 12 or later**. The application source repository remains private.

## Installation and signing status

Download the DMG, open it, and drag KronOS to Applications. A ZIP is also available.
Verify the download against `SHA256SUMS.txt` if desired.

**This preview has an ad-hoc signature. It is not signed with an Apple Developer ID
or notarized by Apple. macOS may block it or require explicit user approval.**
It does not provide the normal trusted installation experience of a notarized
release. Automatic upgrades have not been validated for this preview; use manual
downloads. This is a preview, not a claim of production readiness.

## What changed

- KronOS display branding throughout the desktop, agent UI, and website source.
- Larger shell controls, more consistent icon spacing, visible command search,
  keyboard workspace navigation, and an accessible workspace-view menu.
- A dedicated Control Center entry and clearer agent entry point.
- Bring-your-own-key setup, with local model support and no KronOS account gate.
- Local support reports with preview, copy, refresh, and clear controls in
  Settings > About. No reporting service, service key, or automatic upload.
- Usage telemetry disabled by default for new installs.
- Current bundled MCP/plugin runtimes, required native-binary package checks,
  preserved configuration locations, and third-party license notices.

## Models and privacy

Use your own provider API key, a supported provider sign-in, or a compatible local
model. Your provider bills its own usage and subscriptions. KronOS does not supply
shared inference credits or a shared developer key. Existing local provider
configuration may be detected on your computer.

Reports omit raw error messages, keys, prompts, terminal contents, and personal
file paths. They retain app/platform metadata, failure categories, and locations
in shipped application code. Reports remain local until you choose to share them.
Public GitHub issues require a GitHub account. Review all text and attachments.

## Verification and limits

- TypeScript check, production build, and website build passed.
- 1,713 frontend/Electron tests and 164 MCP tests passed.
- Local diagnostics privacy, persistence, bounded retention, and clear behavior
  were tested. Four build-output guard tests passed.
- The packaged backend and desktop opened in an isolated test profile; welcome,
  workspace entry, browser rendering, and model selection were exercised.
- Shell/support previews were checked at 1280, 1440, and 1920 widths, in light and
  dark appearance, including keyboard use and accessibility settings.

A paid model request, notarized installation on another Mac, automatic upgrade,
and every optional integration were not verified. Intel Mac, Windows, and Linux
installers are not included. Phone support and other Labs capabilities remain
experimental and may require additional runtimes, permissions, or accounts.

Report reproducible issues using Settings > About > Diagnostics & support, or the
[public issue tracker](https://github.com/Ahmedalsadi-1/kronos-releases/issues).
