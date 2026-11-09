# 使用说明

## 适用任务

一节45分钟初中课，前20分钟连续讲授，最后5分钟才做题。

## 准备输入

课堂时间轴、活动记录或转录、教学目标、学生年龄、课堂长度、观察重点、教师自评。使用前先脱敏姓名、联系方式和与任务无关的敏感信息。

## 操作步骤

1. 核对时间记录
2. 标注活动类型
3. 统计占比和切换
4. 对照目标
5. 识别过久/过短环节
6. 提供一个可测试的节奏调整

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
