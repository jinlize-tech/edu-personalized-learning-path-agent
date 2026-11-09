# 使用说明

## 适用任务

一名五年级学生在12周内改善阅读理解与词汇，但每周只有两小时课外时间。

## 准备输入

学生基本情况、学习目标、课程安排、作业/测评摘要、可用时间、教师观察、家长支持条件、周期。使用前先脱敏姓名、联系方式和与任务无关的敏感信息。

## 操作步骤

1. 确认目标与周期
2. 盘点证据
3. 识别关键缺口
4. 设计路径和里程碑
5. 分配任务
6. 阶段复盘
7. 根据证据调整

## 校验命令

```powershell
node scripts/validate_input.js examples/typical_input.json
node scripts/validate_output.js examples/typical_output.json
```

## 状态使用

- `completed`：核心成果完整。
- `completed_with_limits`：只完成可验证部分，并说明受阻范围。
- `needs_input`：缺少关键输入。
- `needs_confirmation`：资料冲突或需人工确认。
- `failed`：工具或计算失败，提供恢复动作。

## 人工确认

业务负责人复核输入事实、关键假设和最终成果适用范围后，成果才可进入正式业务使用。
