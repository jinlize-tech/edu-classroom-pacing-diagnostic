# 课堂节奏与时间分配诊断示例

## 典型场景

一节45分钟初中课，前20分钟连续讲授，最后5分钟才做题。

## 具体示例

系统输出讲授/练习时间结构，建议在12分钟处加入2分钟检索练习，并设下次观察指标。

## 脱敏输入示例

```json
{
  "contract_version": "1.2.0",
  "data_status": "confirmed",
  "contains_sensitive_data": false,
  "requested_output_language": "zh-CN",
  "classroom_timeline": [
    {}
  ],
  "lesson_objectives": [
    {}
  ],
  "lesson_duration": 45,
  "age_group": "学生年龄或年级已核对（脱敏示例）",
  "teacher_self_review": "教师自评已核对（脱敏示例）"
}
```

## 预期处理

1. 运行输入契约校验。
2. 逐项核对输入来源、版本和口径。
3. 按`references/PROFESSIONAL_PLAYBOOK.md`完成专业分析。
4. 输出时间分布图文本、活动序列、目标保障风险等核心成果。
5. 由业务负责人确认输入事实、关键假设和最终成果适用范围后才可作为正式业务结论。

## 不应出现的输出

- 虚构政策、价格、人员、课程或客户事实。
- 以“暂无”“待完善”等占位文本冒充完成。
- 无依据的确定性判断或伪造人工签批。
