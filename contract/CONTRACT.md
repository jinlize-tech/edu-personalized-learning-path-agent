# 输入输出契约

## 输入字段

| 键 | 名称 | 类型 | 必填 |
|---|---|---|---|
| `learner_profile` | 学生概况 | string | 是 |
| `learning_goals` | 阶段目标 | array | 是 |
| `evidence_summary` | 学情证据摘要 | array | 是 |
| `course_schedule` | 课程安排 | array | 是 |
| `available_home_time` | 家庭可用时间 | string | 是 |
| `review_cycle` | 复盘周期 | string | 是 |
| `support_conditions` | 家庭与教师支持条件 | string | 否 |

## 状态

- `completed`：核心成果完整，关键结论人工确认要求满足。
- `completed_with_limits`：至少一项实质成果，说明限制、已完成和受阻范围。
- `needs_input`：必填字段缺失。
- `needs_confirmation`：资料冲突或人工确认未完成。
- `failed`：计算或工具失败。

## 输出

- `个性化路径`：结构化条目数组，不允许空壳或占位文本。
- `阶段目标`：结构化条目数组，不允许空壳或占位文本。
- `任务清单`：结构化条目数组，不允许空壳或占位文本。
- `里程碑`：结构化条目数组，不允许空壳或占位文本。
- `复盘表`：结构化条目数组，不允许空壳或占位文本。
- `调整条件`：结构化条目数组，不允许空壳或占位文本。
- `家长沟通摘要`：结构化条目数组，不允许空壳或占位文本。

完整机器契约见`contract/input.schema.json`、`contract/output.schema.json`和`contract/runtime_contract.json`。
