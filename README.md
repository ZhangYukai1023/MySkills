# MySkills

本服务器上所有 Claude Code Skills 的汇总仓库。

---

## 目录结构

```
skills/
├── installed/               # 已安装的第三方 skills
│   └── python-refactoring/  # Python 代码重构 skills (l-mb/python-refactoring-skills)
├── agents/                  # Agent skills
│   ├── ccpm/                # CCPM 项目流程管理
│   └── find-skill/          # 查找可用 skill
└── marketplace/             # 来自 claude-plugins-official 官方市场
    ├── claude-code-setup/
    ├── claude-md-management/
    ├── cwc-makers/
    ├── example-plugin/
    ├── external/            # 第三方集成插件
    │   ├── asana/           # (plugin only, no skill)
    │   ├── context7/        # (plugin only, no skill)
    │   ├── discord/         # Discord 频道管理
    │   ├── fakechat/        # (plugin only, no skill)
    │   ├── firebase/        # (plugin only, no skill)
    │   ├── github/          # (plugin only, no skill)
    │   ├── gitlab/          # (plugin only, no skill)
    │   ├── greptile/        # (plugin only, no skill)
    │   ├── imessage/        # iMessage 频道管理
    │   ├── laravel-boost/   # (plugin only, no skill)
    │   ├── linear/          # (plugin only, no skill)
    │   ├── playwright/      # (plugin only, no skill)
    │   ├── serena/          # (plugin only, no skill)
    │   ├── telegram/        # Telegram 频道管理
    │   └── terraform/       # (plugin only, no skill)
    ├── frontend-design/
    ├── hookify/
    ├── math-olympiad/
    ├── mcp-server-dev/
    ├── playground/
    ├── plugin-dev/          # 插件/技能开发工具集
    ├── project-artifact/
    ├── session-report/
    └── skill-creator/
```

---

## 1. 已安装的 Python 重构 skills

来源: [l-mb/python-refactoring-skills](https://github.com/l-mb/python-refactoring-skills)

| Skill | 说明 |
|-------|------|
| **py-refactor** | 统筹执行全面重构 |
| **py-complexity** | 降低圈复杂度（radon, lizard） |
| **py-code-health** | 删除死代码、消除重复（vulture, pylint） |
| **py-modernize** | 升级语法和工具链（uv, pyupgrade） |
| **py-quality-setup** | 配置 ruff, mypy 等检查工具 |
| **py-security** | 安全漏洞检测修复（bandit） |
| **py-test-quality** | 提升测试覆盖率和质量（pytest-cov, mutmut） |
| **py-git-hooks** | pre-commit 自动化 |

## 2. Agent skills

| Skill | 说明 |
|-------|------|
| **ccpm** | 基于 PRD 的项目流程管理（Epic → Issue → 并行 Agent → 交付） |
| **find-skill** | 搜索并发现可安装的 Claude Code skills |

## 3. 官方市场 skills (claude-plugins-official)

| 插件 | Skills | 说明 |
|------|--------|------|
| **skill-creator** | skill-creator | 创建、修改、评估新 skill |
| **plugin-dev** | skill-development, hook-development, agent-development, command-development, plugin-structure, plugin-settings, mcp-integration | 插件/skill 全流程开发 |
| **mcp-server-dev** | build-mcp-server, build-mcp-app, build-mcpb | MCP 服务器开发 |
| **frontend-design** | frontend-design | UI/视觉设计指导 |
| **playground** | playground | 创建交互式 HTML 沙箱 |
| **cwc-makers** | m5-onboard, cardputer-buddy | M5Stack/Cardputer 设备开发 |
| **claude-code-setup** | claude-automation-recommender | 推荐 Claude Code 自动化配置 |
| **claude-md-management** | claude-md-improver | CLAUDE.md 文件审计改进 |
| **project-artifact** | project-artifact | 生成项目状态报告 |
| **session-report** | session-report | 生成 Claude Code 会话报告 |
| **math-olympiad** | math-olympiad | 数学奥赛指导 |
| **hookify** | writing-rules | hookify 规则编写 |
| **example-plugin** | example-skill, example-command | Skill 示例参考 |

### 第三方集成 (external)

| 插件 | Skills | 说明 |
|------|--------|------|
| **discord** | access, configure | Discord 频道接入管理 |
| **telegram** | access, configure | Telegram 频道接入管理 |
| **imessage** | access, configure | iMessage 频道接入管理 |
| **asana, context7, fakechat, firebase, github, gitlab, greptile, laravel-boost, linear, playwright, serena, terraform** | (无 skill, 仅 plugin 配置) | 第三方服务插件 |

---

## 更新

```bash
# Python refactoring skills
cd ~/python-refactoring-skills && git pull

# Marketplace plugins (自动同步)
```

收集时间: 2026-06-24
