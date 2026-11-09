# 个性化学习路径规划

围绕一个学习周期建立诊断、目标、任务、里程碑、复盘和调整的多轮路径，不混淆教学建议与正式诊断。

## 适用用户

教学主管、教师、学习管理师、家长沟通人员

## 主要输出

- 个性化路径
- 阶段目标
- 任务清单
- 里程碑
- 复盘表
- 调整条件
- 家长沟通摘要

## 安装

将Agent目录按平台要求导入，并保留`.codebuddy-plugin/plugin.json`、`agents/`、`skills/`与`avatars/`的相对结构。

本地验证：

```powershell
node scripts/validate_input.js examples/typical_input.json
node scripts/validate_output.js examples/typical_output.json
```

## 使用

1. 阅读`USAGE.md`。
2. 按`contract/input.schema.json`准备输入。
3. 调用产品或Agent完成专业处理。
4. 使用`scripts/validate_output.js`检查成果。
5. 高风险结论交由业务负责人确认。

## 边界

- 不使用外部收费API。
- 不依赖其他产品完成核心任务。
- 不自动执行正式审批、退款、人员处罚或系统变更。
- 客户可见内容不包含公司品牌推广或内部研发资料。

## 状态

- 版本：`1.0.0`
- 本地契约与自动化测试：见`test-results/`
- 生成式模型运行：`MODEL_RUNTIME_NOT_VERIFIED`
- WorkBuddy安装、调用、审核、上架：`NOT_EXECUTED`
- 安装包：`dist/edu-personalized-learning-path-agent-v1.0.0.zip`

## 许可证

Apache-2.0。详见`LICENSE`。
