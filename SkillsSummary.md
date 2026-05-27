# OpenCode Skills 管理文档

> 本文件追踪所有已安装和推荐的 OpenCode Skills。每次安装新的 skill 后自动更新。
> 最后更新：2026-05-28

---

## 一、已安装技能（.opencode/skills/）

当前共 **17 个技能**。

### 开发流程（Superpowers 系列）— 14 个

| 技能 | 用途 |
|------|------|
| brainstorming | 需求头脑风暴，生成结构化需求文档 |
| dispatching-parallel-agents | 并行 Agent 调度，多任务并发执行 |
| executing-plans | 按计划逐步执行开发任务 |
| finishing-a-development-branch | 分支完成收尾：检查、提交、合并 |
| receiving-code-review | 接收代码审查反馈并自动修复 |
| requesting-code-review | 自动请求代码审查 |
| subagent-driven-development | 子 Agent 驱动开发：spec → implement → review |
| systematic-debugging | 系统化调试方法：根因分析、分层排查 |
| test-driven-development | TDD 测试驱动开发流程 |
| using-git-worktrees | Git Worktree 并行工作流 |
| using-superpowers | Superpowers 框架使用指南 |
| verification-before-completion | 任务完成前自动验证 |
| writing-plans | 编写结构化开发计划 |
| writing-skills | 编写新的 Skill 的方法论 |

> 来源：[obra/superpowers](https://github.com/obra/superpowers) ⭐209k

### PPT 制作 — 3 个

| 技能 | 来源 | 用途 |
|------|------|------|
| pptx | [Anthropic 官方](https://github.com/anthropics/skills) ⭐141k | 通用 PPT 创建/编辑/模板/html2pptx，最标准最全面 |
| academic-pptx | [Gabberflast](https://github.com/Gabberflast/academic-pptx-skill) ⭐468 | 学术演示：会议报告、论文答辩、讲座，含最佳实践 |
| document-pptx | [appautomaton](https://github.com/appautomaton/document-SKILLs) ⭐96 | PPT 文档增强：OOXML 操作、html2pptx、批量处理 |

---

## 二、热门推荐（未安装，值得关注）

### 强烈推荐

| 排名 | 仓库 | ⭐ | 用途 |
|------|------|------|------|
| 1 | zrt-ai-lab/opencode-skills | 213 | 26 个国内实用技能：飞书/抖音/视频剪辑/小红书 |
| 2 | antongulin/opencode-skill-creator | 103 | 技能开发工具链，eval-driven 自动优化 |
| 3 | alexwwang/aristotle | 14 | AI 错误反思学习系统，5-Why 根因分析 |

### 推荐

| 排名 | 仓库 | ⭐ | 用途 |
|------|------|------|------|
| 4 | FrancoStino/opencode-skills-collection | 25 | 1000+ 技能合集，SkillPointer 懒加载架构 |
| 5 | zenobi-us/opencode-skillful | 302 | 技能懒加载器，支持 XML/JSON/Markdown 格式 |
| 6 | linxuan-sys/opencode-skills-chinese | 134 | Anthropic 官方 17 个技能中文翻译版 |

---

## 三、安装推荐组合

| 用户类型 | 推荐组合 |
|---------|---------|
| **全栈开发** | ✅ superpowers + PPT技能（已装）+ aristotle |
| **内容创作者** | zrt-ai-lab + opencode-skills-collection |
| **技能开发者** | opencode-skill-creator + opencode-skillful |
| **新手入门** | opencode-skills-chinese + superpowers（已装） |

---

## 四、如何安装新技能

```powershell
# 方式一：git clone 到项目 skills 目录
git clone --depth 1 <repo-url> $env:TEMP\new-skill
Copy-Item -Path "$env:TEMP\new-skill\*" -Destination "D:\OpencodeDesktop\.opencode\skills\<skill-name>\" -Recurse

# 方式二：通过 opencode.json 插件
{ "plugin": ["<plugin-name>"] }
```

---

*数据来源：GitHub，实时更新*
