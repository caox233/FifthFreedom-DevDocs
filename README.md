# Fifth Freedom 开发知识库

> 原云执行器及 GitHub 接入已恢复，原未推送成果已保全并推送。
> 本快照绑定已推送源码，固定入口的远端 Git 对象已核对。
> 完整统一包仍受默认存档隐私门禁和未完成集成限制；组件或参考 EXE 不是完整包。

供后续开发者接手的开发过程、代码职责、实现原理与验证边界。不是完整私人聊天、日志或捕获的公开导出。

- [项目源码](https://github.com/caox233/FifthFreedom)
- 本批文档对应源码提交：[`311052da801ee95b085ffbcd95498d5dde5f45ef`](https://github.com/caox233/FifthFreedom/commit/311052da801ee95b085ffbcd95498d5dde5f45ef)
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
- [原生启动许可与父进程续期](docs/tasks/server-10.md)
- [实际服务生命周期与隔离验证](docs/tasks/server-11.md)
- [明确的加密网络配方与观测](docs/tasks/server-12.md)
- [真实隔离加密网络探测](docs/tasks/server-13.md)
- [启动器与原生认证回传](docs/tasks/ui-06.md)
- [原生管道契约与跨语言边界](docs/tasks/ui-06-native-return.md)
- [最终登录与启动准备所有权](docs/tasks/ui-07.md)
- [拥有进程的网络观测与启动许可](docs/tasks/server-14.md)
- [覆盖网络与原生服务的实际组合检查](docs/tasks/server-15.md)
- [原生连接的来源限制与即时撤销](docs/tasks/ui-08.md)
- [历史回放依赖闭包](docs/tasks/vss-replay-closure.md)
- [Windows 自有网络会话与配对源码构建](docs/tasks/ui-09.md)
- [官方 Wintun 输入与有限会话验证](docs/tasks/wintun-retained-session-probe.md)
- [当前 Windows 网卡会话的类型化读取](docs/dependency-patches/easytier-2.6.4-windows-session-read/README.md)
- [实际认证数据接收与会话失效](docs/tasks/authenticated-receive.md)
- [认证接收候选的独立云构建](docs/tasks/authenticated-receive-build.md)
- [自有核心进程的生命周期](docs/tasks/owned-core-process.md)
- [真实诊断文本流及聊天验证边界](docs/tasks/diagnostic-streaming.md)
- [当前 Instance 的拥有进程读取通道](docs/tasks/owned-core-read.md)
- [移除 Packet 捕获依赖的独立源码配方](docs/dependency-patches/easytier-2.6.4-windows-no-packet/README.md)
- [当前认证 Data 挑战及独立构建](docs/tasks/data-challenge-build.md)
- [Linux 观察者权限与当前拥有者许可](docs/tasks/server-16.md)
- [实际 Instance 成员身份与独立 71 项构建](docs/tasks/peer-map-build.md)
- [核心依赖文件的身份与生命周期](docs/tasks/owned-core-dependencies.md)
- [隔离核心配置与默认发现关闭](docs/dependency-patches/easytier-2.6.4-inert-stun/README.md)
- [实际 Windows 核心与网卡验证入口](docs/tasks/owned-core-runtime.md)
- [同作业隔离核心构建与恢复检查](docs/tasks/ci-windows-inert-runtime.md)
- [Windows 启动前防火墙核查](docs/tasks/windows-core-firewall-prerequisite.md)
- [云会话授权恢复与真实续接步骤](docs/tasks/cloud-authentication-recovery.md)
- [MemoryModule 精确上游源码与随包说明](docs/development-reference/fusionfix-loader-memorymodule/README.md)
- [候选产物上传与源码完整性](docs/tasks/ci-artifact-source-closure.md)
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
这是明确的未完成项，不是通过。后续托管运行的结果按准确提交记录在 PROJECT-STATE.json 与 CLOUD-PROGRESS.md；
早先 Windows/Linux 组件通过不能替代最新提交验证，完整包仍受资源门禁阻止。
开发代码由[源码草稿 PR #1](https://github.com/caox233/FifthFreedom/pull/1)审查。

平台当前没有可调用的持续 Goal/调度接口。云端这一轮与 GitHub Actions 不依赖
用户电脑；未来 agent 执行仍需消息或平台唤醒，源码中的下一步记录不是后台调度器。

新实现应同步补充原因、约束、代码入口、实际命令/结果、失败与回滚及待实机范围。
项目仓库的同名文档是开发时的权威版本；此独立知识库按提交更新快照。
不记录密钥、个人账号、聊天正文、原始存档、崩溃转储或图形捕获。

- [统一开发候选包门禁与集中测试](docs/DEVELOPMENT-CANDIDATE-TESTING.md)

- [快速匹配同局调查（needs-triage）](docs/tasks/quick-match-same-session.md)

- [Capture 历史源码独立构建](docs/tasks/capture-reference-build.md)
