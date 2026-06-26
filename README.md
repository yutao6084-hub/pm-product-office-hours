# PM Product Office Hours

一个给创业者、CEO、0-1 产品负责人的 Codex Skill：用“严厉面试官”式问答，把模糊产品想法逼到清晰、可验证、可执行的产品定义包。

它不是普通 PRD 生成器。它会先追问真实用户、具体场景、当前替代方案、验证证据、MVP 取舍和增长假设，然后再输出产品定义、PRD、MVP、路线图、指标、验证计划和风险清单。

## 适合谁

- 创业者 / CEO
- 0-1 产品负责人
- 正在定义新产品的产品经理
- 准备做 MVP、融资材料、立项评审、内部产品决策的人

## 解决什么痛点

很多产品想法的问题不是“不会写 PRD”，而是：

- 用户是谁没说清楚
- 痛点没有证据
- MVP 做得太大
- 需求优先级靠感觉
- 指标体系后补
- 产品定位像口号
- 创始人/CEO 的判断没有被严厉质询

这个 Skill 的目标是先问清楚，再生成文档。

## 能输出什么

默认输出完整产品定义包：

1. 产品定义一页纸
2. PRD 核心草案
3. MVP 范围与非范围
4. 需求优先级表
5. User Stories / Job Stories
6. 用户旅程与核心流程
7. 0-1 验证计划
8. 指标体系
9. 路线图
10. 风险与假设清单
11. CEO / 团队 / 投资人简版叙事
12. 上线后增长与迭代计划

## 安装

把本仓库复制到你的 Codex skills 目录：

```powershell
cd "$env:USERPROFILE\.codex\skills"
git clone https://github.com/YOUR_NAME/pm-product-office-hours.git
```

或手动复制到：

```text
C:\Users\<你的用户名>\.codex\skills\pm-product-office-hours
```

重启 Codex 或开启新会话后即可使用。

## 使用方式

```text
使用 $pm-product-office-hours 帮我把这个产品想法梳理成完整产品定义包。
```

也可以更具体：

```text
使用 $pm-product-office-hours 严格追问我，帮我定义一个面向家长和儿童的体感训练产品，从用户、痛点、MVP、指标到 PRD 都输出。
```

## 工作方式

Skill 会按阶段推进：

1. 判断产品阶段
2. 追问真实用户和具体场景
3. 追问当前替代方案
4. 追问验证证据
5. 收窄 MVP
6. 输出定位与差异化
7. 生成 PRD 与产品定义包
8. 补充验证计划、指标、路线图和增长方案

它会拒绝模糊描述，例如：

- “面向中小企业”
- “体验更好”
- “AI 赋能”
- “市场很大”
- “用户会喜欢”

并追问成：

- 哪一个真实用户？
- 最近一次在什么场景痛？
- 今天怎么解决？
- 为什么不用现有方案？
- 有没有付费、使用、排队、签约或留存证据？
- 两周内只做一个功能，做什么？

## 仓库结构

```text
pm-product-office-hours/
├─ SKILL.md
├─ agents/
│  └─ openai.yaml
├─ references/
│  ├─ phases.md
│  ├─ question-bank.md
│  └─ output-pack.md
├─ examples/
│  └─ sample-prompts.md
├─ ROADMAP.md
├─ CONTRIBUTING.md
└─ LICENSE
```

## 设计原则

- 严厉，不刻薄
- 具体，不空泛
- 先验证，再定义
- 先 MVP，再大愿景
- 明确事实、假设和未知
- 不替 CEO 做必须由本人承担的决策

## License

MIT
