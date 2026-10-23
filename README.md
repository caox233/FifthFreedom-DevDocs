# Fifth Freedom 开发知识库

供后续开发者接手的开发过程、代码职责、实现原理与验证边界。不是完整私人聊天、日志或捕获的公开导出。

- [项目源码](https://github.com/caox233/FifthFreedom)
- 本批文档对应源码提交：[`4a273bf9356ccd3036f67a3e8e7ee1cfce89baeb`](https://github.com/caox233/FifthFreedom/blob/4a273bf9356ccd3036f67a3e8e7ee1cfce89baeb/)
- [开发历史与实现地图](docs/DEVELOPMENT-HISTORY.md)
- [源码入口直达](CODE-MAP.md)
- [14项保留结果与验收边界](docs/ACCEPTANCE.md)
- [剩余 BUG](docs/tasks/remaining-bugs.md)
- [VSS 生命周期云端审计](docs/tasks/vss-lifecycle-audit.md)
- [SCBL3 UI 整合](docs/UI-INTEGRATION.md)
- [Windows LAN / Linux 公网服务端整合](docs/SERVER-INTEGRATION.md)
- [云端交接](docs/CLOUD-HANDOFF.md)
- [云端实现、真实 CI 与验证边界](docs/CLOUD-PROGRESS.md)
- [UI 壳与生命周期实现](docs/tasks/ui-02.md)
- [服务端认证桥接与原生互通](docs/tasks/server-02.md)
- [生产 LAN 生命周期接入](docs/tasks/ui-03.md)
- [原生共享密钥、观察者授权及 Linux 互斥](docs/tasks/server-03.md)
- [HTTPS 控制服务与 Linux 生命周期](docs/tasks/public-transport.md)
- [可复现控制面候选包](docs/tasks/public-candidate.md)
- [公网配置与部署凭据隔离](docs/tasks/ui-04.md)
- [Linux 服务与 Windows 客户端双身份](docs/tasks/server-04.md)
- [真实静态 Public 预检](docs/tasks/server-05.md)
- [原生接口约束](docs/tasks/server-06.md)
- [真实三命名空间隔离验证](docs/tasks/socket-isolation.md)
- [Public 请求源准入](docs/tasks/server-08.md)
- [精确进程所有权与撤销](docs/tasks/server-09.md)
- [受保护会话 HTTPS 客户端](docs/tasks/ui-05.md)
- [公网依赖固定版本与许可门禁](docs/tasks/public-network-dependencies.md)
- [冻结依赖来源与剩余闭包](docs/dependency-closure.md)
- [迁移范围](docs/MIGRATION.md)
- [资源来源与隐私门禁](docs/ASSET-PROVENANCE.md)
- [脱敏历史回归源码参考](docs/development-reference/historical-replays/README.md)

## 状态与维护

这是按准确源码提交同步的云端实现快照，六项迁移目标仍在推进。
Codex 云端负责后续实现；GitHub-hosted Windows/Linux Actions 是常规构建目标；
用户实机反馈单独验收，不把离线通过说成实机通过。

当前公开源码缺少尚在隐私审查门禁内的默认存档，不得声称可以从公开 checkout
独立构建完整包。本地已验证包使用的是本地保留输入。不要通过造假资源或放松 hash
校验绕过门禁。首次 GitHub source-checks 已执行，资源完整性检查因暂存输入缺失而失败，
这是明确的未完成项，不是通过。后续 GitHub Linux LAN、donor 和受保护控制服务构建已通过；
Windows 组件编译、隔离无游戏 UI 自检及回归检查也已通过，完整包仍受资源门禁阻止。
开发代码由[源码草稿 PR #1](https://github.com/caox233/FifthFreedom/pull/1)审查。

平台当前没有可调用的持续 Goal/调度接口。云端这一轮与 GitHub Actions 不依赖
用户电脑；未来 agent 执行仍需消息或平台唤醒，源码中的下一步记录不是后台调度器。

新实现应同步补充原因、约束、代码入口、实际命令/结果、失败与回滚及待实机范围。
项目仓库的同名文档是开发时的权威版本；此独立知识库按提交更新快照。
不记录密钥、个人账号、聊天正文、原始存档、崩溃转储或图形捕获。
