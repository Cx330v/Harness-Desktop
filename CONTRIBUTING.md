# 贡献指南

感谢你帮助改进 Harness Desktop。

## 提交前

1. 先搜索现有 Issue 与 PR，避免重复工作。
2. 不要修改 DeepSeek Harness 的 Agent loop、工具协议、会话格式或 SDK 行为；Desktop 的原则是非侵入式封装。
3. 不提交 API Key、会话、个人目录、安装包、`node_modules`、`target` 或 Runtime 生成目录。
4. 运行 `npm run check`；涉及真实 Runtime 启动时，按项目脚本的显式集成测试说明验证。

## Pull Request

- 一个 PR 只处理一个清晰主题。
- 说明用户可见的变化、测试方式及潜在兼容性影响。
- 涉及权限、插件安装、更新、文件写入或进程管理时，必须说明安全边界与回退方式。
- 不要把“AI 已审计”视为自动合并条件；PR 仍需通过 CI 与维护者审阅。

## 反馈

普通问题和功能建议请使用 Issue 模板。安全漏洞请不要公开提交，按 [SECURITY.md](SECURITY.md) 私下报告。

