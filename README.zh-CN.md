<p align="center">
  <a href="README.md">English</a> ·
  <a href="README.zh-CN.md"><strong>中文</strong></a> ·
  <a href="README.ja.md">日本語</a> ·
  <a href="README.ko.md">한국어</a>
</p>

<h1 align="center">glue-coding-skill：用成熟能力拼出稳定系统</h1>

<p align="center"><strong>一个 Codex Skill：优先复用成熟 SDK / API / 框架 / 平台服务，只写薄胶水层，并用质量门禁收敛 AI 编程结果。</strong></p>

<p align="center">
  <a href="LICENSE"><img alt="MIT" src="https://img.shields.io/badge/license-MIT-2ea44f?style=for-the-badge"></a>
  <img alt="Codex Skill" src="https://img.shields.io/badge/Codex-Skill-111827?style=for-the-badge">
  <img alt="Vibe Coding" src="https://img.shields.io/badge/Vibe%20Coding-工程化-2563eb?style=for-the-badge">
</p>

## 这个 Skill 解决什么问题？

AI 很擅长快速写代码，但也很容易顺手重造轮子：认证、队列、调度、日志、存储、SDK wrapper、工作流引擎……最后项目看起来能跑，维护成本却越来越高。

`glue-coding` 给 Codex 加上一条工程直觉：

> 成熟能力解决通用问题，胶水代码连接业务流程，自研核心能力必须有充分理由。

## 它会引导 Codex 做什么？

- 先找官方能力、平台服务、成熟开源库和事实标准
- 评估维护状态、文档、许可证、安全风险、迁移成本
- 把业务逻辑和外部依赖隔离开
- 只写短、薄、可测、可删的胶水代码
- 补测试、schema、错误处理、重试、监控和回滚路径

## 安装

```powershell
git clone https://github.com/KumiKo2007/glue-coding-skill "$env:USERPROFILE\.codex\skills\glue-coding"
```

然后这样使用：

```text
Use $glue-coding to design this feature with mature capabilities first.
```

## 适合场景

- AI 编程前的技术选型
- 代码审查和架构审查
- 重构 AI 生成的过度自研代码
- API / SDK / 平台能力接入
- 判断该自研、采购、封装还是删除

## 核心循环

```text
需求 -> 成熟能力搜索 -> 方案评估 -> 边界设计 -> 胶水层实现 -> 质量门禁 -> 替换/回滚路径 -> 递归收敛
```

## License

MIT.