# 仓库初始化

日期：2026-10-03（Asia/Shanghai）

## 目标

建立独立 Git 仓库，配置 `main` 和 `develop` 两个工作树，并固定后续开发约定。

## 配置

- 远程名称：`origin`。
- 远程地址：`git@github.com:Alex-WangHT/Awesome-Circuit-Design-Tools.git`。
- 当前项目目录作为 `develop` 工作树。
- `main` 使用 Git 工作树，单独检出到项目内的 `.worktrees/main/`。
- 源码放在 `src/`，项目说明放在 `docs/`，开发节点文档放在 `.develop/`。
- `test/` 仅为空目录，不放置 Git 占位文件。

## 开发限制

本对话不修改 `test/` 内容，不编写测试，不运行测试。

## 初始状态

远程读取成功，初始化时没有远程分支或提交。两个本地分支从同一初始化提交开始；远程推送不属于本次本地初始化操作。

Codex 托管工作树创建受到沙箱账户与桌面账户的 Git 所有权检查限制，因此使用本地 Git 工作树。初始化命令通过 `-c safe.directory=<当前项目绝对路径>` 临时信任本项目，没有修改全局 Git 信任配置。
