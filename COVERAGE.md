# 来源覆盖与验证状态

**状态：提取中。尚未运行 Element Web，也没有进行独立重建。**

## 固定来源

- 项目：[`element-hq/element-web`](https://github.com/element-hq/element-web)
- 发布：[`v1.12.33`](https://github.com/element-hq/element-web/releases/tag/v1.12.33)
- Git 提交：`45671bc88ffe82658619bc523458f3ae3a43bff0`
- 公开仓库元数据：截至 2026-10-29 查询约 13,623 stars；计数会变化，作为来源筛选快照而非配方行为。

## 已观察

- 固定版 README 将 Element 描述为 Matrix 网页与桌面客户端，并称其使用 Matrix JS SDK。
- 发布说明记录该版本的恢复设置、房间切换和其他修复。
- 固定版 `docs/e2ee.md` 说明：当对端账户有已上传密钥时，私聊默认启用加密；创建私密房间时默认加密，但允许用户退出加密设置；密钥恢复会提示用户。
- GitHub 仓库许可元数据为 AGPL-3.0；源码同时包含 AGPL、GPL 与商业许可文件。重建时必须按具体文件和组件检查许可声明，不能假定仓库所有内容使用同一许可。
- 阅读范围限于固定版 README、`package.json`、发布说明、`docs/e2ee.md` 和许可文件；没有克隆或审阅整个约 628 MB 的仓库。

## 未完成范围

尚未完整审阅 Matrix Client-Server API 使用、所有用户流程、消息事件、空间、附件、搜索、通知、设备验证、密钥恢复、客户端发现、桌面封装、浏览器差异、国际化、无障碍、性能、安全审计与完整许可清单。上述项目不能因已写入 `ACCEPTANCE.md` 就视为已验证。

尚未运行上游测试、浏览器验收、独立重建或兼容性测试。`ACCEPTANCE.md` 是未来测试计划；归档和提示词检查只验证配方交付结构，不证明软件能运行或行为完整。
