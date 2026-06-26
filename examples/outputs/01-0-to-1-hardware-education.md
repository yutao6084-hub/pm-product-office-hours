# Golden Example 01: 0-1 Product Definition + Hardware/Education Lens

> Fictional/anonymized example. This demonstrates output structure, not market truth.

## Example prompt

```text
使用 $pm-product-office-hours，并按硬件 + 教育产品模板追问我。
我想做一个给 6-10 岁孩子家庭使用的体感训练硬件 + App。
它通过一个轻量嘴部控制器和手机视觉识别，让孩子站起来做身体动作和口部力量训练。
我们不做医疗诊断，不承诺治疗，只做家庭娱乐训练和训练反馈。
请帮我定义 MVP、PRD、验证计划、指标和家长能看懂的价值。
```

## Product definition one-pager

| Item | Answer |
|---|---|
| Product name | KidMotion Coach |
| Positioning | 亲子体感训练控制器 |
| Target user | 7-10 岁、需要更有趣家庭训练方式的孩子 |
| Buyer | 家长 |
| Painful scene | 家长知道孩子需要规律练习，但传统练习枯燥，孩子坚持不下来，家长也不知道是否有进步 |
| Current substitute | 线下训练课、家长口头监督、视频跟练、普通体感游戏 |
| MVP wedge | 手机摄像头识别 3 个大动作 + 一个轻量嘴部控制动作，驱动现成短互动任务 |
| Core value | 把“必须练”变成“愿意玩”，同时让家长看到基础力量/完成度变化 |
| Differentiation | 手脚身体动作 + 嘴部控制器组合，偏训练反馈而非纯游戏 |
| Why now | 手机端视觉识别成熟、家庭运动娱乐接受度提高、家长愿意为孩子持续练习工具付费 |
| Evidence today | 假设：已有 8 位家长访谈，6 位表示孩子难坚持；无付费证据 |
| Biggest unknown | 孩子是否愿意每周重复使用 3 次以上 |
| Next 2-week action | 做无量产硬件的“假控制器 + 手机视觉”可测 Demo，验证完成率和复玩 |

## MVP scope

### Must build

- 手机 App Demo：摄像头识别站立、下蹲、左右挥手 3 类动作
- 嘴部控制器假硬件：先用现成压力/按压输入模拟“闭唇触发”
- 训练任务：3 个 60 秒互动关卡
- 家长页：显示本周完成次数、动作完成率、嘴部触发成功率
- 非医疗文案：只写训练反馈，不写诊断、治疗、矫正

### Must not build

- 自研游戏大作
- 复杂账号系统
- 医疗报告
- 多儿童长期档案
- 量产级工业设计
- 舌头/嘴部多传感器全功能硬件

### Can fake/manual first

- 家长进步报告可先用本地数据生成
- 嘴部控制器可先用蓝牙键盘/按钮模拟
- 游戏可用网页小游戏或简单互动页替代

### Requires validation before build

- 孩子佩戴舒适度
- 家长是否理解“训练反馈”而非“治疗效果”
- 嘴部控制是否会造成疲劳
- 家庭环境摄像头识别稳定性

## PRD core draft

### Background

家庭训练产品常见问题不是家长不知道要练，而是孩子不愿意长期做、家长缺少可见反馈。本产品希望通过体感互动和轻量嘴部控制器，把训练动作变成可玩任务，并让家长看到完成率和基础能力变化。

Known facts:

- 家长愿意为孩子兴趣、运动、训练类产品付费是可观察趋势。
- 手机摄像头可以在 Demo 阶段完成基础人体动作识别。

Assumptions:

- 目标家庭愿意接受孩子站起来对着手机/平板训练。
- 嘴部控制器足够舒适，不影响孩子继续玩。
- 家长愿意把“完成次数/力度变化”视为有价值反馈。

### Goals

- 让孩子完成 3 个 60 秒训练任务。
- 让家长知道孩子是否完成、是否比基础值有提升。
- 证明“身体动作 + 嘴部控制”的互动方式比普通视频跟练更能提升完成率。

### Non-goals

- 不做疾病诊断。
- 不输出医疗建议。
- 不替代医生、治疗师或线下专业训练。
- 不做大规模游戏内容平台。

### Core flow

1. 家长打开 App。
2. 孩子站到摄像头前。
3. App 做 20 秒基础校准。
4. 孩子完成 3 个互动任务。
5. App 记录动作完成率和嘴部触发成功率。
6. 家长看到本次反馈和本周趋势。

### Functional requirements

| Priority | Module | Requirement | User scene | Acceptance criteria |
|---|---|---|---|---|
| P0 | Camera interaction | Recognize 3 large body actions | Child plays standing interaction | 80%+ recognition in well-lit room |
| P0 | Mouth trigger | Detect one binary mouth action | Child triggers game action | Trigger latency < 200ms in demo |
| P0 | Calibration | Establish baseline per session | Parent wants fair difficulty | Calibration completed in < 30s |
| P0 | Parent feedback | Show completion and trend | Parent checks whether child practiced | Parent can understand result within 10s |
| P1 | Reward path | Stars and weekly streaks | Child needs motivation | Child sees immediate reward after each task |
| P2 | Multiple profiles | Support siblings | Family has more than one child | Not in MVP |

### Edge cases

- Room too dark
- Camera distance too close
- Child leaves frame
- Child refuses mouth controller
- Device falls off
- Parent misreads training feedback as treatment effect

## Validation plan

| Assumption | Test | Target users | Success threshold | Timeline | Owner |
|---|---|---|---|---|---|
| Child will complete tasks | 5-family home demo | 7-10 year-old children | 4/5 children finish 3 tasks | 2 weeks | Founder |
| Mouth control is tolerable | 10-minute comfort test | Same children | 80% report no discomfort / parent observes no rejection | 2 weeks | Hardware |
| Parent sees value | Parent interview after demo | Parents | 4/5 can explain feedback value | 2 weeks | PM |
| Vision recognition is enough for demo | In-home lighting test | 5 homes | 80%+ action recognition | 1 week | Engineering |

## Metrics framework

- North star: weekly completed training sessions per child
- Activation: child completes first 3-task session
- Retention: child completes 3 sessions in 7 days
- Quality: action recognition success rate, mouth trigger success rate
- Safety guardrail: discomfort reports, abnormal dropout, device fall-off
- Parent value: parent understands report without explanation

## Roadmap

- Week 0-2: fake hardware + camera interaction demo
- Week 3-6: 10-family private beta, comfort and repeat-use testing
- Week 7-12: improved controller prototype, parent report iteration
- Quarter 2+: evaluate real hardware BOM and limited pilot production

## CEO / team / investor narrative

### CEO internal decision memo

Do not build a game company yet. Build a proof that children will repeatedly complete short training tasks when body movement and mouth control are combined, and that parents value simple feedback.

### Team execution brief

The first milestone is not content richness. It is a 2-week Demo proving: camera recognition works, one mouth trigger works, children complete tasks, parents understand feedback.

### Investor-style summary

We are testing a family training controller category that combines body interaction and oral-motor-like control input for entertainment training. The wedge is not medical treatment; it is repeatable family training behavior with parent-visible progress.

## Self-check

| Item | Score / 5 | Issue | Repair / next action |
|---|---:|---|---|
| User clarity | 4 | Age and buyer clear, but exact family profile still broad | Interview 10 target parents |
| Pain evidence | 2 | Current evidence is mostly interview assumption | Run paid pre-order or deposit test |
| Substitute clarity | 4 | Substitutes are clear | Compare against video follow-along |
| MVP narrowness | 4 | MVP is narrow enough for Demo | Resist adding more sensors |
| Requirement buildability | 4 | P0 can be built | Engineering spike for camera latency |
| Metrics | 4 | Retention and completion defined | Add instrumentation plan |
| Differentiation | 3 | Differentiation plausible but not proven | Test against plain body-only interaction |
| Business model | 2 | Pricing/BOM unknown | Build BOM and willingness-to-pay test |
| Risk honesty | 5 | Non-medical and comfort risks explicit | Keep warnings in parent-facing copy |

### Severe red flags

- Do not imply medical diagnosis or treatment.
- Do not commit to custom hardware before proving repeat use.

### Questions to ask users next

- “你现在如何让孩子坚持练习？”
- “你愿意为一个能让孩子每周练 3 次的工具付多少钱？”
- “你看到什么反馈才相信孩子有进步？”
