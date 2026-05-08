# Zunisper — public releases

This repo only hosts the published builds of **Zunisper**, the local-first
dictation app. The source code lives in a private repo; this one exists so
anyone can download the `.app` without a GitHub account.

## Download

Latest stable build is on the [Releases](https://github.com/dplopezsioux/zunisper-releases/releases/latest)
page.

### macOS (Apple Silicon, M1/M2/M3/M4)

1. Download `Zunisper-<version>-macos-aarch64.zip` from the latest release.
2. Unzip — you get `Zunisper.app`.
3. Move it to `/Applications` (or wherever you keep apps).
4. The first launch is blocked by macOS Gatekeeper because the build is not
   yet code-signed/notarized. To open it the first time:
   - Right-click `Zunisper.app` → **Open** → confirm the "unidentified
     developer" dialog.
   - From then on, double-click works normally.
5. The first time you record, macOS will ask for microphone permission.
   Grant it — without it, transcription will return silence.

Intel Macs and Windows are not supported in this build.

## What it does

- Local dictation with whisper.cpp (model `ggml-medium`, ~1.5 GB,
  downloaded on first run).
- Notes + folders, drag-and-drop, recording → "Save as note" flow.
- Optional sync to a Zunisper account — sign in from the **Account**
  panel. The web companion at <https://app.zunisper.com> lets you read
  your notes from any browser.
- Logout fully invalidates the SSO session.

## Support the project

Zunisper is built and maintained by one person. If it saves you time and
you'd like to chip in for the next bag of coffee:

[**☕ Buy me a coffee**](https://buymeacoffee.com/dplopez)

Or scan the QR with your phone:

<img src="qr-code.png" alt="buymeacoffee.com/dplopez QR" width="180" />
