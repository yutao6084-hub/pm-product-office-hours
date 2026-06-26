# Contributing

欢迎改进这个 Skill。适合贡献的方向：

- 更好的追问问题
- 更强的行业模板
- 更清晰的输出结构
- 更严格的产品定义自检规则
- 英文版本
- 示例对话和示例输出

## 修改原则

- 保持 `SKILL.md` 精简。
- 把详细内容放到 `references/`。
- 不要把 Skill 改成普通鼓励型 PRD 生成器。
- 不要接受模糊产品描述。
- 不要让 AI 编造用户证据、收入、留存或市场数据。

## 校验

修改后运行：

```powershell
$env:PYTHONUTF8='1'
python "$env:USERPROFILE\.codex\skills\.system\skill-creator\scripts\quick_validate.py" .
```

看到 `Skill is valid!` 后再提交。
