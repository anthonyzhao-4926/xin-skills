---
name: xin-git-commit-flow
description: git 提交工作流快捷命令，启动subagent，生成commit message, 然后push
disable-model-invocation: true
context: fork
agent: git-commit-flow
---

使用 git-commit-flow subagent 执行 git 提交。主要工作是按照规范生成commit message, 然后push