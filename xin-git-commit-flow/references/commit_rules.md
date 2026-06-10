# commit message 规范
生成的commit message 必须遵守如下规范
| 字段 | 说明 | 详情 |
|------|------|------|
| **格式** | `<type>(<scope>): <subject>` | 例如 `refactor(auth): 重构登录态校验逻辑` |
| **type** | `feat` | 新功能 |
| | `fix` | 修复 bug |
| | `docs` | 仅文档（README、CHANGELOG 等） |
| | `style` | 仅格式（空格、缩进、分号），不改逻辑 |
| | `refactor` | 重构，无新功能也无修复 |
| | `perf` | 性能 / 体验优化 |
| | `chore` | 构建流程、依赖、工具 |
| | `test` | 测试相关 |
| | `revert` | 回滚 |
| **scope** | 可选 | 改动范围，例如 `auth` / `model` / `api` |
| **subject** | 简短中文描述 | 一句话说清这次 commit 做了什么 |

