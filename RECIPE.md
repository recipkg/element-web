# Element Web：Matrix 网页客户端配方

```toml
format = "recipkg/1"

[package]
name = "element-web"
version = "0.1.0"
kind = "software"
description = "基于 Matrix 的开源网页通讯客户端，覆盖账户、房间、消息、端到端加密和客户端配置。"
entry = "BUILD_PROMPT.md"

[dependencies.quality]
git = "https://github.com/recipkg/recipkg.git"
rev = "7f05425ae9843b7e8ce15cb80917977eedb36bdd"
subdir = "recipes/software-quality"

[dependencies.design]
git = "https://github.com/recipkg/design-directions.git"
rev = "6fdba350d1effa2d50dc0185095bb91ca7a699ee"
```

## 目标

重建 Element Web 浏览器客户端。它是 Matrix 互通通讯产品的客户端，不是 Matrix homeserver。客户端应通过配置连接可替换的 homeserver；协议服务及其数据存储属于外部运行前提。

范围包括浏览器中的账户登录、房间和私聊、消息时间线、实时同步、端到端加密与密钥恢复、通知、设置、无障碍和自托管配置。固定上游版本内的 SDK 与共享前端包应作为同一 monorepo 的内部组件处理，不能误写成外部运行服务。桌面外壳及平台专属功能需另行确认边界。

## 依赖用途

`quality` 提供错误处理、状态一致性、安全边界、自动化验收和性能测量合同；它是构建指导材料，不是 Element Web 的运行时依赖。`design` 提供按场景选择的视觉与交互设计方法；不得把它误解为某个厂商的原始设计系统。Matrix homeserver、推送网关和第三方集成是可选或外部服务，只有在对应功能范围内才需要。

来源提交、许可证、已观察事实与未知范围见 `SOURCES.md` 和 `COVERAGE.md`。本配方仍在提取，不代表已完成软件重建。
