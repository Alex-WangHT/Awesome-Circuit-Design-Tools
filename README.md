# Awesome Circuit Design Tools

电路与 PCB 设计工具项目。

## 仓库与分支

- 远程仓库：`git@github.com:Alex-WangHT/Awesome-Circuit-Design-Tools.git`
- `main`：主分支，使用独立工作树。
- `develop`：开发分支，当前项目目录及后续开发均基于此分支。
- 合并至 `main` 或向远程推送时，按当次任务的授权执行。

## 目录约定

```text
.
├── .gitignore
├── README.md
├── src/          # 项目源码
├── test/         # 预留测试目录；本对话不写入任何文件
├── docs/         # 项目使用与说明文档
└── .develop/     # 开发节点记录与开发约定
```

Git 不跟踪空目录。`test/` 仅在本地建立，不放置占位文件；新检出的工作树可创建空目录，但本对话不修改其内容。

## 本对话的开发约束

1. 所有后续开发以 `develop` 为基础，不直接在 `main` 上开发。
2. 不创建、修改、删除或移动 `test/` 下的文件。
3. 不编写测试代码，不运行任何测试命令或测试套件。
4. 开发节点文档统一写入 `.develop/`；允许使用只读 Git 状态与差异检查确认变更范围。

详细约定见 [.develop/CONVENTIONS.md](.develop/CONVENTIONS.md)。
