# Lumo Router — download and install

A local model-routing app for Codex and Claude Code.

## [⬇ Download for Mac — Apple Silicon](https://github.com/volyapers17/lumo-router-downloads/releases/latest/download/Lumo-Router-macOS-arm64.dmg)

**Mac with an M1 / M2 / M3 / M4 or newer Apple Silicon chip · macOS 14+**

Installers for Intel Macs, Windows, and Linux are not available here yet.
To check your Mac, open the Apple menu → **About This Mac** → **Chip**.

### Install in 3 steps

1. **Download and open the DMG.** Drag **Lumo Router.app** into **Applications**.
2. **Open Lumo Router from Applications.** Its icon appears in the menu bar near the clock; there may be no separate Dock window.
3. **Connect your own account or API key**, then connect Codex / Claude through the Lumo panel. Connecting backs up and changes the selected client's settings; follow the prompts and restart the client if requested.

**No Git, Node.js, Terminal, repository cloning, or Lumo website signup required.**
Codex / Claude must be installed separately. API access requires your own key and is billed separately from subscriptions.

### Important: before your first launch

This is an **experimental test build**, signed ad hoc, **without an Apple Developer ID signature or Apple notarization**.
macOS may block the first launch. Only if you trust this source and have verified the file:
after attempting to launch it, open **System Settings → Privacy & Security**;
if **Open Anyway** is offered, use it to confirm the launch.
Do not disable Gatekeeper, antivirus software, or system protection.
If macOS reports malware or offers no Open Anyway button, stop and report the issue.

ChatGPT-plan mode is experimental: availability and compatibility depend on your account and client.
Tests using local API mocks do not guarantee compatibility with a live account.

### Updates and disconnecting

- To update, download the new DMG, choose **Quit** in Lumo, replace the app in Applications, and open it again. Automatic updates are not available yet.
- Your settings stay on your Mac in `~/.lumo-router`; this repository does not contain them.
- Use **Disconnect** in Lumo to restore the client's standard configuration.
- For emergency Codex recovery, copy **both apps** from the DMG into the same Applications folder, then launch **Restore Standard Codex.app**. The recovery app asks for confirmation and does not automatically overwrite conflicting settings.

### Other downloads

- [ZIP instead of DMG](https://github.com/volyapers17/lumo-router-downloads/releases/latest/download/Lumo-Router-macOS-arm64.zip)
- [All versions and release notes](https://github.com/volyapers17/lumo-router-downloads/releases)
- [SHA-256 checksums for the latest version](https://github.com/volyapers17/lumo-router-downloads/releases/latest/download/SHA256SUMS.txt)
- [Report an issue](https://github.com/volyapers17/lumo-router-downloads/issues/new)

Checksums help verify file integrity; they are not a substitute for an Apple signature.
Optional Terminal command for comparison: `shasum -a 256 ~/Downloads/Lumo-Router-macOS-arm64.dmg`.

This public repository contains only instructions and installers. Source code,
personal keys, OAuth tokens, local settings, and request history are not published here.
