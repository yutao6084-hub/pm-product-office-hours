# PM Product Office Hours

> Strict product-definition Office Hours skill for founders, CEOs, product managers, and 0-1 builders.

一个面向创业者、CEO、产品经理的 Codex Skill：用“严厉面试官”式问答，把模糊产品想法、PRD 草稿、融资叙事或增长问题，拆成可验证、可执行、可评审的产品定义包。

## 30 秒看懂

它不是普通 PRD 生成器。它会先追问：

- 真实用户是谁？
- 最近一次具体痛点发生在哪里？
- 今天用什么替代方案？
- 有什么证据，而不是创始人脑补？
- MVP 能不能砍到一个最小楔子？
- 指标、验收标准、边界场景是否清楚？
- 投资人会怎么质疑市场、护城河、商业模式和团队优势？

然后再输出 PRD、MVP、路线图、验证计划、指标体系、自检报告，以及 DOCX/PPT/飞书文档可用结构。

## 当前能力

| 能力 | 说明 |
|---|---|
| 行业模板 | 支持 SaaS、硬件、AI Agent、消费 App、教育等产品的专属追问、指标和风险检查 |
| 一小时 PRD 评审 | 用户已有 PRD 时，先审漏洞、缺失决策、MVP 范围、指标和可交付性，再给修正版 |
| 投资人视角质询 | 从市场、护城河、商业模式、团队优势、证据和 90 天里程碑进行严厉挑战 |
| 多格式输出 | 支持 Markdown、DOCX-ready、PPT 10 页大纲、飞书/Lark 文档块结构 |
| 自检器 | 检查是否脑补证据、MVP 是否过大、指标是否缺失、差异化是否空泛 |
| 黄金样例 | 提供 3 个匿名化真实感案例，展示完整输出效果 |

## 适合谁

- 创业者 / CEO
- 0-1 产品负责人
- 正在定义新产品的产品经理
- 准备做 MVP、融资材料、立项评审、内部产品决策的人
- 已有 PRD，但需要严厉审查漏洞的人

## 安装

把本仓库复制到你的 Codex skills 目录：

```powershell
cd "$env:USERPROFILE\.codex\skills"
git clone https://github.com/yutao6084-hub/pm-product-office-hours.git
```

或手动复制到：

```text
C:\Users\<你的用户名>\.codex\skills\pm-product-office-hours
```

重启 Codex 或开启新会话后即可使用。

## 更新到最新版

如果你已经安装过：

```powershell
cd "$env:USERPROFILE\.codex\skills\pm-product-office-hours"
git pull
```

如果 Codex 没有自动触发这个 Skill，直接在提示词里显式写：

```text
使用 $pm-product-office-hours ...
```

## 最快使用

### 1. 定义一个新产品

```text
使用 $pm-product-office-hours。请严格追问我，帮我把这个产品想法梳理成完整产品定义包。
```

### 2. 评审已有 PRD

```text
使用 $pm-product-office-hours 的一小时 PRD 评审模式。我会贴一份 PRD，请你先审漏洞，再输出修正版。
```

### 3. 用投资人视角质询

```text
使用 $pm-product-office-hours 的投资人质询模式。请挑战我的市场、护城河、商业模式、团队优势和 90 天验证计划。
```

### 4. 使用行业模板

```text
使用 $pm-product-office-hours，并按硬件 + 教育产品模板追问我。请特别检查 BOM、儿童体验、家长价值、训练反馈和非医疗化表达。
```

### 5. 输出多格式

```text
使用 $pm-product-office-hours。请输出 Markdown 产品定义包，并附上 DOCX-ready 结构、PPT 10 页大纲和飞书文档块结构。
```

更多示例见 [examples/sample-prompts.md](examples/sample-prompts.md)。

## 直接看输出效果

如果你不想先读说明，可以直接看这 3 个黄金样例：

| 示例 | 展示能力 |
|---|---|
| [儿童家庭训练硬件 + App](examples/outputs/01-0-to-1-hardware-education.md) | 0-1 产品定义、硬件/教育行业模板、MVP、PRD、自检 |
| [AI 销售跟进 SaaS PRD 评审](examples/outputs/02-prd-review-saas.md) | 一小时 PRD 评审、漏洞清单、范围裁剪、修正版 PRD |
| [跨境电商运营 AI Agent 投资人质询](examples/outputs/03-investor-challenge-ai-agent.md) | 投资人视角、AI Agent 边界、护城河、90 天验证计划 |

样例索引见 [examples/outputs/README.md](examples/outputs/README.md)。

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
13. 自检评分与修正建议

如果你明确要求多格式输出，还可以附加：

- DOCX-ready 结构
- PPT 10 页大纲
- 飞书/Lark 文档块结构

## 工作模式

| 类型 | 适用场景 |
|---|---|
| 主模式：0-1 Product Definition | 从想法、原型或模糊方向开始定义产品 |
| 主模式：One-Hour PRD Review | 已有 PRD/需求列表，需要严厉评审 |
| 主模式：Investor Challenge | 准备融资、路演、董事会或 CEO 级产品质询 |
| 辅助层：Industry Template | SaaS、硬件、AI Agent、消费 App、教育等垂直产品 |
| 辅助层：Output Formatting | 需要 Markdown、DOCX、PPT、飞书文档结构 |
| 质量门：Self-Check | 检查证据、MVP、指标、差异化、商业模式是否站得住 |

## 内部测试

本仓库包含一份公开的内部测试报告：

[tests/internal-test-report.md](tests/internal-test-report.md)

测试覆盖：

- 0-1 新产品定义
- 已有 PRD 评审
- 投资人视角质询
- 硬件 + 教育行业模板
- 多格式输出
- 自检器
- 引用文件完整性和 Skill 结构校验

## 边界说明

- 这个 Skill 不会替你编造用户证据、付费数据或市场规模。
- 这个 Skill 不直接承诺医疗、法律、金融等高风险结论。
- 如果要求生成 DOCX/PPT/飞书文档，是否能真正创建文件取决于当前 Codex 环境是否有对应工具；否则会输出 copy-ready 结构。

## 仓库结构

```text
pm-product-office-hours/
├─ SKILL.md
├─ agents/
│  └─ openai.yaml
├─ references/
│  ├─ phases.md
│  ├─ question-bank.md
│  ├─ output-pack.md
│  ├─ industry-templates.md
│  ├─ prd-review-mode.md
│  ├─ investor-challenge.md
│  ├─ output-formats.md
│  └─ self-checker.md
├─ examples/
│  ├─ sample-prompts.md
│  └─ outputs/
│     ├─ 01-0-to-1-hardware-education.md
│     ├─ 02-prd-review-saas.md
│     └─ 03-investor-challenge-ai-agent.md
├─ tests/
│  └─ internal-test-report.md
├─ CHANGELOG.md
├─ RELEASE_NOTES.md
├─ ROADMAP.md
├─ CONTRIBUTING.md
└─ LICENSE
```

## 推荐 GitHub Topics

```text
product-management, prd, startup, codex-skill, mvp, product-strategy, founder, product-discovery, product-review, investor-readiness
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
