# HopClaw

[简体中文](./README.zh-CN.md)

HopClaw is a governed agent runtime for teams operating through chat, browser,
desktop, and HTTP surfaces.

This repository is the official public GitHub entry for HopClaw. It is used for
releases, installation guidance, documentation links, security reporting
instructions, and public product updates.

Public source code is not available in this repository yet.

## Quick Links

- Website: https://hopclaw.com
- Documentation: https://hopclaw.com/docs
- Releases: https://github.com/hopclaw/hopclaw/releases
- Issues: https://github.com/hopclaw/hopclaw/issues
- Install (macOS / Linux): `curl -fsSL https://hopclaw.com/install.sh | sh`
- Install (Windows PowerShell): `irm https://hopclaw.com/install.ps1 | iex`

## Status

- HopClaw is available to use today through release binaries.
- This repository does not contain the runtime source tree.
- Tagged releases, checksums, and update notes are the primary artifacts
  published here.
- Security-sensitive reports should follow [SECURITY.md](./SECURITY.md), not
  public issues.

## What HopClaw Does

- governs long-running agent runs and session lifecycle
- provides approvals, audit trails, artifacts, and operator-friendly reporting
- supports chat, browser, desktop, and HTTP execution surfaces
- exposes built-in tools plus extension points for skills, channels, and hosted
  capabilities

## Install

### macOS / Linux

```sh
curl -fsSL https://hopclaw.com/install.sh | sh
```

### Windows PowerShell

```powershell
irm https://hopclaw.com/install.ps1 | iex
```

### Guided Onboarding

macOS / Linux:

```sh
curl -fsSL https://hopclaw.com/install.sh | HOPCLAW_INSTALL_RUN_ONBOARD=1 sh
```

Windows PowerShell:

```powershell
$env:HOPCLAW_INSTALL_RUN_ONBOARD='1'; irm https://hopclaw.com/install.ps1 | iex
```

## Reporting Bugs

Before opening a bug:

1. Run `hopclaw doctor`.
2. If possible, generate a redacted bundle with `hopclaw bug-report`.
3. Open an issue with the bug template and include version, platform,
   reproduction steps, and logs.

If the problem is security-sensitive, do not file a public issue. Use the
process in [SECURITY.md](./SECURITY.md).

## Contributing

This repository is not accepting source code contributions for the private core
runtime yet. For the current contribution boundary and the types of feedback
that are useful now, see [CONTRIBUTING.md](./CONTRIBUTING.md).

## Why The Source Is Not Public Yet

HopClaw is currently distributed as release binaries while the product surface,
licensing position, and support process continue to be tightened. This
repository exists to give users a stable canonical GitHub entry before a
broader source release decision is made.

## Chinese Summary

HopClaw 是一个面向团队的 Agent Runtime，覆盖聊天、浏览器、桌面和 HTTP
运行面。这个仓库是 HopClaw 的官方 GitHub 公开入口，用于发布版本、提供安装
说明、链接文档、承接安全说明以及同步产品更新。目前本仓库暂不公开运行时
源码。

Chinese details: [README.zh-CN.md](./README.zh-CN.md)
