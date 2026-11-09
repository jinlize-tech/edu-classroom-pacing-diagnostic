# 输入输出契约

## 输入字段

| 键 | 名称 | 类型 | 必填 |
|---|---|---|---|
| `classroom_timeline` | 课堂时间轴 | array | 是 |
| `lesson_objectives` | 课堂目标 | array | 是 |
| `lesson_duration` | 课堂时长 | integer | 是 |
| `age_group` | 学生年龄或年级 | string | 是 |
| `teacher_self_review` | 教师自评 | string | 否 |

## 状态

- `completed`：核心成果完整，关键结论人工确认要求满足。
- `completed_with_limits`：至少一项实质成果，说明限制、已完成和受阻范围。
- `needs_input`：必填字段缺失。
- `needs_confirmation`：资料冲突或人工确认未完成。
- `failed`：计算或工具失败。

## 输出

- `时间分布图文本`：结构化条目数组，不允许空壳或占位文本。
- `活动序列`：结构化条目数组，不允许空壳或占位文本。
- `过渡耗时`：结构化条目数组，不允许空壳或占位文本。
- `目标保障风险`：结构化条目数组，不允许空壳或占位文本。
- `改进实验`：结构化条目数组，不允许空壳或占位文本。
- `复盘指标`：结构化条目数组，不允许空壳或占位文本。

完整机器契约见`contract/input.schema.json`、`contract/output.schema.json`和`contract/runtime_contract.json`。
