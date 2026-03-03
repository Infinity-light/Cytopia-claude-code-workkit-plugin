# Changelog

## [2.2.0] - 2026-03-03

### Changed
- **重大变更**: 重组为独立插件仓库结构
- 移除子目录 `plugins/workflow-kit/`，所有内容移至根目录
- 使用 URL 源安装替代本地路径源，修复 `.claude-plugin` 目录未复制问题
- 更新 repository URL 为独立仓库地址

### Migration Guide (from v2.1.0)
1. 卸载旧版本: `/plugin uninstall workflow-kit@infinity-workflows`
2. 添加新 marketplace: `/plugin marketplace add Infinity-light/cytopia-marketplace`
3. 安装新版本: `/plugin install workflow-kit@cytopia-marketplace`
4. 重启 Claude Code

## [2.1.0] - 2026-03-03

### Added
- 迁移到 Claude Code Plugin Marketplace 格式
- 新增 marketplace.json 定义 infinity-workflows marketplace
- 新增 plugin.json 定义 workflow-kit plugin
- 新增 migrate.py 热迁移脚本，支持用户无缝迁移
- 新增 validate.py 契约验证脚本

### Changed
- 所有 skills 从 ~/.claude/skills/ 迁移到 plugin 内部结构
- 支持版本化安装和自动更新
- CLAUDE.md 作为 plugin 提示词加载

### Included Skills
- deploy
- diagnosis
- discovery
- documentation-update
- execution
- key-reader
- learned
- planning
- skills-updater
- verification
- smart-fetch
- ui-ux-pro-max
- frontend-design
- vue-best-practices

## [2.0.0] - 2026-02-28

### Initial Release
- 完整的 Claude Code 工作流套件
- 7 个核心阶段技能
- 6 个辅助技能
