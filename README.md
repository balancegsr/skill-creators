# Skill Creators

> **MethodCraft** series — 把经过验证的方法论编译为可执行的 AI Skill

一组 Skill Creator（生成器），根据你的项目上下文生成定制化的 AI Skill。

每个 Creator 做同一件事：用 2-3 轮对话了解你的情况，然后生成一个 SKILL.md——在你的整个项目过程中持续引导，从规划到执行到收尾。

## 家族成员

| Creator | 做什么 | 典型场景 | 状态 |
|---|---|---|---|
| [learning](./learning/) | 生成学习项目 Skill | "系统学 Rust" / "一周搞懂 RAG" | ✅ v1.0 |
| design | 生成设计项目 Skill | "设计 XX 产品核心流程" | 🔲 开发中 |
| build | 生成构建项目 Skill | "用 Next.js 搭 XX" / "开发一个 Skill" | 🔲 计划中 |

## 工作原理

```
你的项目上下文 → Creator（2-3 轮对话）→ 定制 SKILL.md → 持续引导你的项目
```

Creator 是一次性的生成工具。它的产物——项目级 Skill——才是长期陪你的东西。

## 共享设计

三个 Creator 共享同一套交互框架和设计原则：

- **结构化对话收集**：必答变量 3-5 个，可选变量被动捕获，不像填表
- **预览-迭代-交付**：先给你看生成物预览，满意再交付，随时可提修改
- **两种模式**：轻量模式（短期聚焦）和完整模式（长期系统），覆盖范围不同但引导质量一致
- **文件自动管理**：生成的 Skill 自动追踪进度、保存笔记、管理上下文，你不需要手动操作文件
- **严禁删除用户文件**：所有"归档"都是读取优先级的调整，原始文件始终保留

## 兼容性

主要为 [OpenClaw](https://github.com/nicepkg/OpenClaw) 设计，同时兼容能操作本地文件系统的 AI Agent 产品（Claude Code、WorkBuddy、CodeBuddy 等）。所有指令使用描述性语言，不依赖特定平台 API。

## 安装

各 Creator 独立安装。进入对应子目录查看说明：

- [learning/README.md](./learning/README.md) — 学习项目 Skill Creator

## License

MIT
