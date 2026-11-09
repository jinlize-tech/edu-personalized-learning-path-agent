# 个性化学习路径规划示例

## 典型场景

一名五年级学生在12周内改善阅读理解与词汇，但每周只有两小时课外时间。

## 具体示例

Agent 设计每周阅读、词汇和复述任务的梯度，每三周根据测评和教师观察复盘，避免一次性堆满任务。

## 脱敏输入示例

```json
{
  "contract_version": "1.2.0",
  "data_status": "confirmed",
  "contains_sensitive_data": false,
  "requested_output_language": "zh-CN",
  "learner_profile": "学生概况已核对（脱敏示例）",
  "learning_goals": [
    {}
  ],
  "evidence_summary": [
    {}
  ],
  "course_schedule": [
    {}
  ],
  "available_home_time": "家庭可用时间已核对（脱敏示例）",
  "review_cycle": "复盘周期已核对（脱敏示例）",
  "support_conditions": "家庭与教师支持条件已核对（脱敏示例）",
  "resume_mode": "new"
}
```

## 预期处理

1. 运行输入契约校验。
2. 逐项核对输入来源、版本和口径。
3. 按`references/PROFESSIONAL_PLAYBOOK.md`完成专业分析。
4. 输出个性化路径、阶段目标、里程碑等核心成果。
5. 由业务负责人确认输入事实、关键假设和最终成果适用范围后才可作为正式业务结论。

## 不应出现的输出

- 虚构政策、价格、人员、课程或客户事实。
- 以“暂无”“待完善”等占位文本冒充完成。
- 无依据的确定性判断或伪造人工签批。
