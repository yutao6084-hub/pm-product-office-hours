# Industry Templates

Select one or more lenses when the product category is visible. Do not force every template question into the interview; use the template to catch domain-specific blind spots.

## SaaS

Key split:

- User vs buyer vs admin
- Individual workflow vs team workflow
- SMB self-serve vs enterprise sales

Must ask:

- “谁每天用？谁付钱？谁有权采购？”
- “这个工作流发生频率是多少？每天不用会不会流失？”
- “客户今天用什么系统替代？Excel、Notion、飞书、CRM、ERP、内部系统？”
- “数据从哪里来？需要接哪些系统？没有集成时能否先人工导入？”

Metrics:

- Activation: first successful workflow completed
- Retention: weekly/monthly repeated workflow
- Expansion: seats, usage, modules, data volume
- Revenue: MRR/ARR, gross retention, net retention

Red flags:

- 只说“提效”，没有具体节省时间或提升转化
- 买单人与使用者完全分裂但没有销售路径
- 依赖重集成，MVP 却没有手工替代方案

## Hardware

Key split:

- Device value vs companion app value
- Prototype vs mass production
- BOM vs retail price vs channel margin
- Reliability, safety, certification, returns

Must ask:

- “硬件不可替代的软件价值是什么？为什么不能只做 App？”
- “首版 BOM 上限是多少？目标零售价是多少？毛利空间够不够？”
- “哪些传感器/结构/材料决定体验？”
- “量产前最可能失败的是精度、舒适度、寿命、供应链、认证，还是售后？”
- “如果硬件延期，是否能用假硬件、现成硬件或手机传感器先验证？”

Metrics:

- Setup success rate
- First-use completion rate
- Device accuracy / latency / battery / durability
- Return rate, defect rate, support ticket rate
- Companion app retention

Red flags:

- 先讲愿景，不讲 BOM 和量产风险
- 首版硬件承担太多未经验证的功能
- 舒适度/安全/儿童使用场景没有验证计划

## AI Agent

Key split:

- Copilot vs autonomous agent
- One-shot task vs recurring workflow
- Human approval vs full automation
- Data access vs trust boundary

Must ask:

- “Agent 具体替用户完成哪一个任务？输入是什么，输出是什么？”
- “失败的代价是什么？错一次用户会不会立刻弃用？”
- “哪些步骤必须人审？哪些可以自动执行？”
- “如何评价 Agent 做得好？有没有标准答案、人工评分或线上行为指标？”

Metrics:

- Task completion rate
- Human correction rate
- Hallucination / unsafe action rate
- Time saved per successful task
- Repeat usage by workflow

Red flags:

- “AI 赋能”但没有明确任务边界
- 没有 eval，只靠主观感觉
- Agent 能写入真实系统但没有权限和回滚设计

## Consumer App

Key split:

- One-time novelty vs repeat habit
- Content loop, social loop, utility loop, reward loop
- Organic acquisition vs paid acquisition

Must ask:

- “用户为什么今天就打开？为什么明天还打开？”
- “第一次获得价值发生在第几秒/第几步？”
- “用户会主动分享给谁？分享内容是什么？”
- “如果没有广告投放，第一批 1000 个用户从哪里来？”

Metrics:

- D1/D7/D30 retention
- Activation event
- Session frequency
- Share/invite rate
- CAC, LTV, pay conversion

Red flags:

- 只靠“好玩/好看”，没有留存机制
- 获客渠道是空泛的“做小红书/抖音”
- 没有定义核心行为

## Education

Key split:

- Learner vs parent vs teacher vs school buyer
- Engagement vs learning outcome
- Curriculum fit vs entertainment
- Safety and age appropriateness

Must ask:

- “谁使用？谁监督？谁付钱？谁判断有效？”
- “训练/学习结果如何被观察？家长能看到什么物理或行为层面的提升？”
- “孩子为什么愿意持续做？奖励机制会不会压过真正训练目标？”
- “是否涉及医疗、诊断、治疗等敏感表述？如果不做，文案必须如何避开？”

Metrics:

- Training completion rate
- Repeat sessions per week
- Skill baseline vs follow-up change
- Parent-reported confidence / observed improvement
- Safety incidents / discomfort / dropout

Red flags:

- 对儿童承诺治疗效果
- 家长价值不清晰，只强调孩子喜欢
- 训练强度、疲劳、舒适度没有边界
