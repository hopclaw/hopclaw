# HopClaw

[English README](./README.md)

HopClaw 是一个面向团队的 Agent Runtime，覆盖聊天、浏览器、桌面和 HTTP
运行面。

这个仓库是 HopClaw 的官方 GitHub 公开入口，用于发布版本、提供安装说明、
链接文档、承接安全说明以及同步产品更新。

当前这个仓库暂不公开运行时源码。

## 快速链接

- 官网：https://hopclaw.com
- 文档：https://hopclaw.com/docs
- Releases：https://github.com/hopclaw/hopclaw/releases
- Issues：https://github.com/hopclaw/hopclaw/issues
- 安装（macOS / Linux）：`curl -fsSL https://hopclaw.com/install.sh | sh`
- 安装（Windows PowerShell）：`irm https://hopclaw.com/install.ps1 | iex`

## 当前定位

- HopClaw 当前已经可以通过 release 二进制使用。
- 这个仓库不是运行时源码仓库。
- 这里主要承载版本发布、校验信息、安装入口和公开更新。
- 安全问题请走 [SECURITY.md](./SECURITY.md) 中的私密流程，不要发公开 issue。

## HopClaw 做什么

- 管理长生命周期 agent 的 run 与 session
- 提供审批、审计、artifact 和面向运维的可追踪能力
- 覆盖 chat、browser、desktop 与 HTTP 运行面
- 提供内置工具，以及 skills、channels、hosted capabilities 的扩展边界

## 安装

### macOS / Linux

```sh
curl -fsSL https://hopclaw.com/install.sh | sh
```

### Windows PowerShell

```powershell
irm https://hopclaw.com/install.ps1 | iex
```

### 引导式首次配置

macOS / Linux：

```sh
curl -fsSL https://hopclaw.com/install.sh | HOPCLAW_INSTALL_RUN_ONBOARD=1 sh
```

Windows PowerShell：

```powershell
$env:HOPCLAW_INSTALL_RUN_ONBOARD='1'; irm https://hopclaw.com/install.ps1 | iex
```

## Bug 反馈建议

提交问题前，建议先做这几步：

1. 运行 `hopclaw doctor`
2. 如果方便，执行 `hopclaw bug-report` 生成脱敏后的问题包
3. 使用仓库里的 bug 模板提交，并附上版本号、平台、复现步骤和日志

如果问题涉及安全，请不要提交公开 issue，改走 [SECURITY.md](./SECURITY.md)
中的流程。

## 贡献说明

当前这个仓库暂不接收针对私有核心运行时的源码贡献。关于目前接受什么类型的
反馈，以及哪些参与方式最有价值，请看 [CONTRIBUTING.md](./CONTRIBUTING.md)。

## 为什么现在还不公开源码

目前 HopClaw 仍以 release 二进制方式分发，产品边界、许可证策略和支持流程
还在继续收紧和稳定。这个仓库的目的，是先为用户提供一个稳定的官方 GitHub
入口，再决定更广泛的源码开放节奏。
