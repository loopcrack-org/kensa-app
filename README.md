# Kensa

**AI-powered pull-request review, on your desktop.**

Kensa is a desktop app that reviews GitHub, GitLab and Bitbucket pull requests
with a team of configurable AI specialist agents (architecture, security, error
handling, testing, code quality — or agents you define). It presents structured
findings in a visual diff UI, learns your repository's conventions, and never
auto-publishes anything without you.

This repository hosts **downloads and changelogs only** — the application source
is developed in a private repository.

## Download

Grab the latest version from the **[Releases page](https://github.com/loopcrack-org/kensa-releases/releases/latest)**:

| Platform | File | Notes |
| --- | --- | --- |
| macOS (Apple Silicon) | `Kensa-<version>-arm64.dmg` | Signed & notarized — open normally |
| macOS (Intel) | `Kensa-<version>-x64.dmg` | Signed & notarized — open normally |
| Windows 10/11 (x64) | `Kensa-Setup-<version>-x64.exe` | Unsigned for now: SmartScreen will warn — click **More info → Run anyway** |
| Linux (x64) | `Kensa-<version>-x86_64.AppImage` | `chmod +x` the file, then run it |

The app updates itself automatically from this repository after the first install.

## How it works

1. **Connect** your GitHub / GitLab / Bitbucket account (OAuth or PAT — Kensa
   talks to the provider APIs directly; no CLI tools required).
2. **Pick a PR** — or open one straight from the browser with the
   [Kensa Companion extension](https://chromewebstore.google.com/) ("Open in Kensa" on any GitHub PR).
3. **Review** — specialist agents analyze the diff in parallel and return
   structured findings you can triage, discuss, and publish as a review.
4. **Learn** — Kensa builds a digest of your repo's architecture and
   conventions so reviews get sharper over time.

Kensa uses your own AI subscription (Claude CLI) — your code goes to your AI
provider and the git host you already use, nowhere else.

## Requirements

- [Claude Code CLI](https://claude.com/claude-code) installed and authenticated
- A GitHub, GitLab or Bitbucket account

## Changelog

See [CHANGELOG.md](./CHANGELOG.md).

## Issues & feedback

This repository does not accept source contributions. For bug reports and
feedback, open an issue here.
