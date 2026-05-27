# OpenCode Skills 热门推荐（2026年5月）

> 基于 GitHub 近期热门项目调研，总结最值得安装的 OpenCode Skills。

---

## 零、已安装（本次）

### obra/superpowers ⭐209k

**已安装到 `.opencode/skills/`**，共 14 个技能：

```
brainstorming              — 需求头脑风暴
dispatching-parallel-agents — 并行 Agent 调度
executing-plans            — 计划执行
finishing-a-development-branch — 分支完成收尾
receiving-code-review      — 接收代码审查
requesting-code-review     — 请求代码审查
subagent-driven-development — 子Agent 驱动开发
systematic-debugging       — 系统化调试
test-driven-development    — 测试驱动开发
using-git-worktrees        — Git Worktree 工作流
using-superpowers          — Superpowers 使用指南
verification-before-completion — 完成前验证
writing-plans              — 编写计划
writing-skills             — 编写技能
```

---

## 一、强烈推荐（必装）

### 1. zrt-ai-lab/opencode-skills ⭐213

**国内实用场景最丰富的技能集**，共 26 个 Skill，覆盖六大方向：

| 分类 | 技能 | 用途 |
|------|------|------|
| 内容创作 | 图像生成/视频生成/短视频文案/小红书笔记 | 自媒体内容一键生产 |
| 自动发布 | 抖音/视频号 | 内容分发自动化 |
| 视频剪辑 | videocut 系列（5个协同） | 完整口播视频制作流程 |
| 飞书集成 | 文档读写/群聊记录/定时提醒 | 办公效率提升 |
| 开发工具 | 数据库查询/CSV分析/日志分析/MCP开发 | 数据分析与工具开发 |
| Agent调度 | uni-agent | 跨协议统一调度 |

**安装方式：**
```bash
git clone https://github.com/zrt-ai-lab/opencode-skills
cp -r opencode-skills/* ~/.opencode/skills/
```

> 如果你做内容创作或社交媒体运营，这是必装合集。飞书、抖音、视频号全打通。

---

### 2. antongulin/opencode-skill-creator ⭐103

**技能开发必备工具链**，基于 Anthropic 官方 skill-creator 移植到 TypeScript。

核心能力：
- 自动生成评测集，测试技能触发准确率
- 5 轮迭代自动优化技能描述质量
- 可视化评测审查器（HTML）
- 基准测试（方差分析）

**安装方式：**
```bash
npx opencode-skill-creator install --global
```

> 如果你要创建自己的 OpenCode 技能，这是最专业的选择。

---

### 3. alexwwang/aristotle ⭐14

**AI 错误反思与学习系统**，独树一帜的"从错误中学习"机制。

核心能力：
- `/aristotle` 命令触发错误反思
- 5-Why 根因分析（8 类错误模式）
- 自动生成改进规则（pending → staging → verified 生命周期）
- 双输出：用户级 + 项目级规则
- 中英双语支持
- 20 个 Git MCP 工具，1000+ 测试用例

**安装方式（Windows）：**
```bash
git clone https://github.com/alexwwang/aristotle
powershell install.ps1
```

> 希望 AI 持续改进、建立系统化反思机制？这是目前最完善的开源方案。

---

## 二、推荐安装

### 4. FrancoStino/opencode-skills-collection ⭐25

**1000+ 技能的超级合集**，目前规模最大的技能库。

特色：
- SkillPointer 智能指针架构：仅暴露 ~35 个轻量指针，避免启动时加载全部技能
- 自然语言自动匹配技能
- 风险等级过滤器（可排除高风险技能）
- 支持 beta 版本频道

**安装方式：**
```bash
# 在 opencode.json 中添加
{ "plugin": ["opencode-skills-collection@latest"] }
```

> 1000+ 技能取之不尽，SkillPointer 架构避免 token 爆炸。

---

### 5. zenobi-us/opencode-skillful ⭐302

**智能技能加载器**，差异化优势显著。

特色：
- 懒加载：按需加载指定技能，不预加载全部
- 模型格式定制：支持 XML / JSON / Markdown 渲染
- 安全资源访问：预索引路径，防路径遍历

**安装方式：**
```bash
# 在 opencode.json 中添加
{ "plugins": ["@zenobius/opencode-skillful"] }
```

> 如果你技能众多但不想耗尽 context window，这个懒加载方案非常合适。

---

### 6. linxuan-sys/opencode-skills-chinese ⭐134

**Anthropic 官方技能集的中文翻译版**，17 个 Skill 全汉化：

算法艺术、架构故障排查、画布设计、图表生成、代码审查、
文档协著、DOCX、前端设计、MCP 构建器、PDF、Playwright CLI、
PPTX、技能创建器、系统调试、主题工厂、XLSX

**安装方式：**
```bash
git clone https://github.com/linxuan-sys/opencode-skills-chinese
cp -r opencode-skills-chinese/* ~/.opencode/skills/
```

> 官方技能英文读起来费劲？这个中文版直接可用。

---

## 三、已弃用（跳过）

### ~~malhashemi/opencode-skills ⭐488~~

早期 Skills 插件，已被 OpenCode v1.0.190 原生 skill 功能取代，仅作历史参考。

---

## 安装推荐组合

| 用户类型 | 推荐组合 |
|---------|---------|
| **内容创作者** | zrt-ai-lab（必装）+ opencode-skills-collection |
| **技能开发者** | opencode-skill-creator（必装）+ opencode-skillful |
| **团队/长期项目** | aristotle（必装）+ opencode-skills-collection |
| **新手入门** | opencode-skills-chinese + zrt-ai-lab |
| **全都要** | 全部安装 |

---

*数据来源：GitHub，截至 2026-05-27*
