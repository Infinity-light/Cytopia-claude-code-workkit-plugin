# Workflow Kit for Claude Code

完整的 Claude Code 工作流套件，提供 discovery → planning → execution → diagnosis → verification → documentation-update → deploy 全阶段支持。

## 安装

通过 Cytopia Marketplace 安装：

```bash
/plugin marketplace add Infinity-light/cytopia-marketplace
/plugin install workflow-kit@cytopia-marketplace
```

或直接通过 GitHub URL 安装：

```bash
/plugin install https://github.com/Infinity-light/claude-workflow-kit
```

## 包含的技能

| 技能 | 用途 | 触发命令 |
|------|------|----------|
| discovery | 需求调研、信息收集 | /discovery |
| planning | 架构设计、方案规划 | /planning |
| execution | 代码实现 | /execution |
| diagnosis | 问题诊断、故障排查 | /diagnosis |
| verification | 部署验证、质量检查 | /verification |
| documentation-update | 文档更新 | /documentation-update |
| deploy | 部署同步 | /deploy |

## 辅助技能

| 技能 | 用途 |
|------|------|
| key-reader | 读取密钥、配置文件 |
| smart-fetch | 智能网页抓取 |
| ui-ux-pro-max | UI/UX 设计规范 |
| frontend-design | 前端组件设计 |
| vue-best-practices | Vue.js 最佳实践 |
| skills-updater | 更新/创建 Skill |

## 工作流程

```
discovery → planning → execution → verification → documentation-update
                 ↓           ↓
              diagnosis ←────┘
```

## 使用规范

1. **始终先加载 Skill**，再开始工作
2. **不要在 Skill 外自行发挥**
3. **遇到问题先回查 Skill**
4. **完成工作后更新 Skill**（如有不足）

## 版本信息

- **Plugin**: workflow-kit
- **Version**: 2.1.0
- **Author**: Infinity-light
- **Repository**: https://github.com/Infinity-light/claude-workflow-kit

## 许可证

MIT
