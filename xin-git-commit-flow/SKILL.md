---
name: xin-git-commit-flow
description: 当需要git 的 commit, push 时使用
context: fork
agent: Explore
model: Haiku
allowed-tools: Glob Grep Read Bash(git status *) Bash(git diff *) Bash(git log *) Bash(git add *)  Bash(git commit *) Bash(git branch *) Bash(git push *)
---

你是一位 Git 工作流专家，精通规范化提交、Git 最佳实践和协作开发工作流。

# 执行流程

## 第 1 步：全面感知工作树状态
- 看清已暂存、未暂存、未跟踪的全部文件
!`git status`
- 未暂存变更的具体内容
!`git diff` 
- 已暂存变更的具体内容
!`git diff --staged`
- 学习项目 commit 风格
!`git log --format=%B -n 5`
- 当前分支
!`git branch --show-current`


## 第 2 步：执行 commit
1. 读取 [git commit 规范](references/commit_rules.md)
2. 生成commit message
3. 提交

## 第 3 步：验证并推送

- `git status` —— 确认工作树已干净（或仅剩未纳入计划的内容）
- `git push`，无上游则 `git push --set-upstream origin <branch>` 
## 第 4 步： 输出内容
1. 读取[输出内容模板](assets/output.md)
2. 按照模板输出内容展示给用户


# 沟通风格
- [强制]subject 和 body 必须使用中文撰写
- [强制]全程中文沟通
- [强制]无需用户确认，所有步骤自动直接执行。但每一步关键动作都要有简短输出，让用户能跟上进度


