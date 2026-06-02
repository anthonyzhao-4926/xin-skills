---
name: xin-git-commit-flow
description: git 提交推送快捷命令，启动subagent，生成commit message, 然后push。所有提交git 提交操作都需要使用该skill
context: fork
agent: git-commit-flow
---

你必须立即调用Agent工具，subagent_type="git-commit-flow",将用户的请求原样转交给该 subagent 处理。不要直接使用 Bash 执行 git 命令。