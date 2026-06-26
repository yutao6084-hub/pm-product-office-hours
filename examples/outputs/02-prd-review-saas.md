# Golden Example 02: One-Hour PRD Review for SaaS

> Fictional/anonymized example. This demonstrates PRD review mode.

## Example prompt

```text
使用 $pm-product-office-hours 的一小时 PRD 评审模式。
以下是我的 PRD 摘要：
我们要做一个 AI 销售跟进助手，帮助销售自动总结客户会议、生成下一步任务、提醒跟进。
目标用户是 B2B 销售团队。首版包括会议录音、转写、摘要、CRM 同步、自动发邮件、销售主管看板、团队排行榜。
请先审漏洞，不要直接重写。
```

## Verdict

- Decision: Needs rewrite
- Top reason: 目标用户和 MVP 过宽。当前 PRD 把销售个人、销售主管、CRM 管理员的需求混在一起，且 P0 范围接近完整产品而不是可验证首版。

## Scorecard

| Area | Score / 10 | Main issue | Required fix |
|---|---:|---|---|
| User clarity | 5 | “B2B 销售团队”太宽 | 先选 SDR、AE 或销售主管其中一个 |
| Pain evidence | 4 | 没有证明跟进失败造成损失 | 补充真实丢单/延迟跟进案例 |
| MVP scope | 3 | P0 含录音、转写、CRM、邮件、看板、排行榜 | 砍到“会议后 5 分钟生成下一步任务” |
| Requirement buildability | 5 | 功能名清楚，验收标准缺失 | 给每个 P0 加输入、输出、成功标准 |
| Metrics | 4 | 只有使用量，没有结果指标 | 加跟进任务完成率、跟进时延 |
| Edge cases | 3 | 未覆盖转写错误、客户隐私、CRM 权限 | 加失败和权限场景 |
| Business model | 5 | 没有 buyer 和预算来源 | 明确销售主管/RevOps 是否付费 |
| Delivery readiness | 4 | 工程需要大量猜测 | 先定义数据流和最小集成方式 |

## Top 10 product risks

1. 首版范围过大，导致 8 周内无法验证核心价值。
2. 自动发邮件存在信任风险，销售可能不敢让 AI 直接触达客户。
3. CRM 同步会被权限、字段、流程差异拖慢。
4. 销售主管看板不是个人销售的第一价值点。
5. 排行榜可能引发团队抵触，不是核心问题。
6. 会议摘要准确但不代表销售会跟进。
7. 没有明确目标会议类型：首次需求沟通、方案会、报价会、续约会？
8. 没有定义“好摘要”和“好下一步任务”的评价标准。
9. 没有处理客户隐私、录音授权和企业合规。
10. 没有证明销售愿意改变现有 CRM/笔记习惯。

## Missing decisions

- CEO/Product must decide:
  - 首版服务 AE 还是销售主管？
  - 自动发邮件是否从 MVP 中移除？
  - CRM 是真同步，还是先复制粘贴/导出？
- User research must answer:
  - 销售今天会后多久跟进？
  - 哪类会议最容易丢下一步？
  - 销售不跟进是忘了、懒、怕写错，还是 CRM 流程太重？
- Engineering must estimate:
  - 转写服务成本
  - 摘要质量评估方式
  - CRM 最小集成成本

## Scope cut

### Keep

- 上传/导入会议文本
- 生成 3 条结构化下一步任务
- 销售手动确认任务
- 生成可复制的跟进邮件草稿
- 本地/轻量任务列表

### Cut

- 自动发送邮件
- 销售主管看板
- 团队排行榜
- 多 CRM 深度同步
- 会议录音全链路

### Fake/manual first

- CRM 同步先用复制按钮
- 转写先允许用户上传已有文本
- 邮件发送先只生成草稿

## Rewritten core PRD skeleton

### Product thesis

帮助 B2B AE 在客户会议后 5 分钟内生成可确认的下一步任务和跟进草稿，减少跟进延迟和遗漏。

### Primary user

B2B AE，每周有 10+ 次客户会议，当前通过手写笔记、CRM note、飞书/Slack 私聊记录下一步。

### Core scene

客户会议结束后，AE 需要快速整理客户需求、承诺事项、下一步动作，并在当天发出跟进。

### P0 requirements

| Priority | Requirement | Acceptance criteria |
|---|---|---|
| P0 | Import meeting transcript/text | User can paste or upload text within 30 seconds |
| P0 | Generate structured summary | Output includes customer pain, decision maker, objections, next step |
| P0 | Generate next-step tasks | Each task has owner, action, deadline, confidence |
| P0 | User confirmation | AE can accept/edit/reject each task |
| P0 | Follow-up draft | Draft is copy-ready, not auto-sent |

### Metrics

- Activation: first imported meeting creates at least one accepted task
- Core value: time from meeting end to follow-up task confirmation
- Retention: weekly active AE with 3+ processed meetings
- Quality: accepted task rate, edited task rate, rejected task rate
- Business: team pilot conversion to paid workspace

## Next 7 days

1. Interview 5 AEs about last missed follow-up.
2. Collect 10 anonymized meeting notes.
3. Build paste-text prototype, no recording, no CRM.
4. Run task quality evaluation with 3 sales users.
5. Decide if CRM copy/export is enough for beta.

## Self-check

| Item | Score / 5 | Issue | Repair / next action |
|---|---:|---|---|
| User clarity | 4 | AE selected, but company size unclear | Choose SMB SaaS AE or enterprise AE |
| Pain evidence | 2 | No quantitative loss proof | Ask users for missed follow-up examples |
| MVP narrowness | 5 | Scope now narrow | Keep CRM and auto-send out |
| Requirement buildability | 4 | P0 is buildable | Add detailed prompt/eval spec |
| Metrics | 4 | Behavior metrics defined | Add baseline follow-up delay |
| Differentiation | 3 | Still close to generic AI note taker | Focus on sales next-step quality |
| Risk honesty | 5 | Trust and integration risks explicit | Validate with pilot users |
