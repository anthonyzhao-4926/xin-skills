---
name: xin-git-commit-flow
description: git 提交推送快捷命令，启动subagent，生成commit message, 然后push。所有提交git 提交操作都需要使用该skill
context: fork
agent: git-commit-flow
---

你必须立即调用 Agent 工具，subagent_type="git-commit-flow"，处理 git 提交推送流程。                                                            
                                                                                                                                             
参数转交规则：                                                                                                                                 
如果用户提供了具体请求（skill 触发时附带了参数），将该请求原样转交给 subagent。                                                              
如果用户没有提供具体请求（仅触发了 skill 本身、参数为空），默认转交以下任务："分析当前 git 工作树的全部改动，按本仓库历史 commit 风格生成简洁的 commit message，暂存相关文件后创建 commit，并推送到当前分支对应的远端。完成后简要汇报 commit hash、message、推送结果。"                     
不要直接使用 Bash 执行 git 命令，所有 git 操作均由 git-commit-flow subagent 执行。