# 贡献指南

感谢你对 A+H 股价差分析框架的关注！欢迎通过以下方式贡献。

## 🐛 报告问题

提交 Issue 时请包含：
- 使用的框架版本（见 SKILL.md 页眉）
- 分析的标的代码
- 遇到问题的具体步骤
- 期望结果 vs 实际结果

## 💡 建议改进

### 框架逻辑
- 新增成因维度（当前四层：制度/筹码/基本面/汇率）
- 调整信号阈值（需附历史回测数据）
- 新增催化剂类型模板

### 新的市场适配
当前框架针对 A+H 双重上市。如需适配其他双重上市市场：
- ADR 与本土股（如日本 ADR vs 东证所）
- 欧美交叉上市（如 London vs NYSE）
- 其他新兴市场双重上市

请提交 Issue 说明适配场景，讨论确认后提交 PR。

## 📝 提交规范

### Commit Message

```
<type>: <description>

[type] feat | fix | docs | refactor | test | chore
```

示例：
- `feat: 新增 Step 4 板块溢价参照系自动获取`
- `fix: 修正汇率换算方向（HKD→CNY 而非 CNY→HKD）`
- `docs: 补充中芯国际 A/H 分析案例`

### PR 流程
1. Fork 本仓库
2. 创建分支：`git checkout -b feat/your-feature`
3. 提交更改：`git commit -m "feat: ..."`
4. 推送：`git push origin feat/your-feature`
5. 提交 Pull Request

## ✅ 校验要求

修改框架逻辑时，需附至少一个实战案例的复跑校验记录（参照 `references/huahong-case-2026.md` 第 8 节格式）。

## 📊 新案例贡献

欢迎贡献新的 A+H 标的分析案例：
1. 按 SKILL.md 七步流程完成分析
2. 保存至 `references/` 目录，命名格式：`{公司简称}-case-{YYYYMM}.md`
3. 包含完整的轨迹数据、四层诊断、校验记录

---

> 所有贡献者将在 CHANGELOG.md 中署名感谢。
