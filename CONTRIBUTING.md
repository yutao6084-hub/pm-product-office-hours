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

## 贡献黄金样例

欢迎贡献 `examples/outputs/` 下的样例输出。样例应该帮助新用户快速看懂这个 Skill 的真实效果。

要求：

- 使用匿名化或虚构案例，不要暴露真实客户、真实收入、融资材料、内部策略。
- 在文件开头说明是 fictional/anonymized example。
- 至少包含：输入 prompt、核心输出、自检结果。
- 明确标注事实、假设和未知。
- 不要使用医疗、法律、金融等高风险承诺性表述。
- 控制长度，让读者 3-5 分钟能读完核心内容。

推荐覆盖这些类型：

- 0-1 Product Definition
- One-Hour PRD Review
- Investor Challenge
- Industry Template
- Multi-format output
- Self-check

## 校验

修改后运行：

```powershell
$env:PYTHONUTF8='1'
python "$env:USERPROFILE\.codex\skills\.system\skill-creator\scripts\quick_validate.py" .
```

看到 `Skill is valid!` 后再提交。
